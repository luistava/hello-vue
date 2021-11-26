<template>
    <div>
        <p v-html="header"></p>
        <h2>{{name}}</h2>
        
        <h3>{{ok?"Yes":"No"}}</h3>
        <button v-on:click="hello">Click</button>
    </div>
</template>


<script>
export default {
    name:"TemplateComponents",
    data(){
        return{
            name:"Mr.Tavares",
            ok:true,
            header:"<h1>Template in vue js</h1>"
        }
    },methods:{
        hello(){
            this.ok = !this.ok
        }
    }
}
</script>