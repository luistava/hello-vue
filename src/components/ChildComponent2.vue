<template>
    <div>
        <h1>Child Component</h1>
        <h3 v-for="user in users" :key="user.name" >{{ user.name }}

        </h3>
    </div>
</template>

<script>
export default {
    name:"ChildComponent2",
    props:['users']
}
</script>

<style>
#app {
    font-family: Avenir, Arial, Helvetica, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing:grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
}
</style>