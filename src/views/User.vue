<template>
    <div >
        <h1>This is a {{ username }}'s page </h1>
    </div>
</template>

<script>
export default {
    props: ['username']
}
</script>