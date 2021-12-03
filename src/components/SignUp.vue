<template>
    <div>
        <input type="text" placeholder="username" v-model="signupForm.username"> <br> <br>
        <input type="password" placeholder="password" v-model="signupForm.password"> <br> <br>
        <p>Hobbies</p>
        <input type="checkbox" value="travel" id="travel" v-model="signupForm.hobbies">
        <label for="travel"> Travel</label><br>
        <input type="checkbox" value="sports" id="sports" v-model="signupForm.hobbies">
        <label for="sports"> Sports</label><br><br>
        <p>Gender</p>
        <input type="radio" value="male" id="male" v-model="signupForm.gender">
        <label for="male"> Male</label><br>
        <input type="radio" value="female" id="female" v-model="signupForm.gender">
        <label for="female"> Female</label><br>
        <br><br><button v-on:click="registerForm">Register</button>

    </div>
</template>

<script>
export default {
    name:"SignUp",
    data(){
        return {
            signupForm:{
                username:null,
                password:null,
                hobbies:[],
                gender:null
            }
        }
    },
    methods:{
        registerForm(){
            console.log(this.signupForm)
        }
    }
}
</script>