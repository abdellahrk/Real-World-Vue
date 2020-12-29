<template>
    <div id="nav">
        <router-link to="/">Real World Events</router-link> 
        <nav>
        <router-link :to="{ name: 'event-list' }">List</router-link> |
        <router-link :to="{ name: 'event-create'}">Create</router-link> |
        <router-link :to="{ name: 'user', params: { username: 'Ramadan'}}">Ramadan</router-link>
        </nav>
    </div>
</template>

<script>
export default {
    
}
</script>