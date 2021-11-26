<template>
    <div>
        <h1>Bind Component</h1>
        <h1>{{ message }}</h1>
        <input type="text" v-model="message">
    </div>
</template>

<script>
export default {
    name:"DataBind",
    data(){
        return{
            message:"Hi"
        }
    }
}
</script>