<template>
  <div>
      <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
      <h1>Props in Vue</h1>
      <child-component-2 v-bind:users=users />
      
  </div>  
  
</template>

<script>

import ChildComponent2 from './components/ChildComponent2.vue'
export default {
  name: 'App',
    components:{
      ChildComponent2
    },
    data(){
      return {
        users:[
          {name:'Luis',email:'luis@mail.com'},
          {name:'Antonio',email:'antonio@mail.com'},
          {name:'Artur',email:'artur@mail.com'},
          {name:'Ariel',email:'ariel@mail.com'},
        ]
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
