<template>
    <div>
        <h1 v-if="show"> Condition rendering in Vue</h1>
        <h1 v-else> Else side</h1>
        <button v-on:click="display">Toogle</button>
        <h1>For loop in Vue js</h1>
        <table border="2px">
            <tr>
                <td>ID</td><td>Name</td><td>Email</td>
            </tr>
            <tr v-for="user in users" :key="user.id">
                
                <td>{{user.id}}</td>
                <td>{{user.name}}</td>
                <td>{{user.email}}</td>
            </tr>
        </table>
    </div>
    
    
</template>

<script>
export default {
    name:'HomeComponent',
    props:{
        data:String,
        msg:String
    },data(){
        return{
            users: [
                {id:1,name:'Luis',email:'luistava127@gmail.com'},
                {id:2,name:'Antonio',email:'antonio@gmail.com'},
                {id:3,name:'Ariel',email:'ariel@gmail.com'},
                {id:4,name:'Artur',email:'artur@gmail.com'}
            ]
        }
    }
    /*methods:{
        hello(item){
            //alert("hello function called")
            console.warn(item)
        }
    }*/
    ,data2(){
        return{
            show:false
        }
    },
    methods:{
        display(){
            this.show=!this.show
        }
    }
}
</script>