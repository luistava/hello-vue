<template>
    <div>
        <input type="text" v-model="loginForm.username" placeholder="Username"> <br> <br>
        <input type="password" v-model="loginForm.password" placeholder="Password"> <br> <br> 
        <button v-on:click="getLogin">Login</button>
    </div>
</template>

<script>
export default {
    name:"LoginComp",
    data(){
        return {
            loginForm:{
                username:null,
                password:null
            }
        }
    },
    methods:{
        getLogin(){
            console.log("getLogin Called",this.loginForm)
        }
    }
}
</script>