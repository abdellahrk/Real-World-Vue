<template>
    <div >
        <div class="event-card">
            <router-link :to="{ name: 'event-show', params: { id : 1}}">
                <span>@{{ event.time}} on {{ event.date }}</span>
                <h4>{{ event.title }}</h4>
                <span>{{ event.attendees.length }} attending</span>
            </router-link> 
        </div>
    </div>
</template>

<script>
    export default {
        data() {
            return {
                event: {
                    id : 1,
                    title: 'Park Cleanup',
                    date: 'Mon, 28 Jan, 2020',
                    time: '6:48',
                    attendees: [
                        {id: 'abc123', name: 'Abdellah'},
                        {id: 'def321', name: 'Fadil'}
                    ]
                }
            }
        },
    }
</script>

<style scoped>
.event-card{
  border-width: 2px;
  border-color: black;
  
}
    h4 {
        color: green
    }
</style>