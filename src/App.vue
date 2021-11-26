<template>
  <div>
      <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
      <h1>Send props Child to Parent</h1>
      <h1>{{ title }}</h1>
      <child-component v-on:ChangeTitle="updateTitleText($event)"/>
      
  </div>  
  
</template>

<script>

import ChildComponent from './components/ChildComponent.vue'
export default {
  name: 'App',
    components:{
      ChildComponent
    },
    data(){
      return{
        title:"Child to parent Data"
      }
    },
    methods:{
      updateTitleText(title){
        this.title=title
      }
    }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
