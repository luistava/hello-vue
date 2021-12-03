<template>
  <div>
      <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
      <h1>Make Form in Vue</h1> <br>
      <login-comp/>
      
  </div>  
  
</template>

<script>

import LoginComp from './components/LoginComponent.vue'
export default {
  name: 'App',
    components:{
      LoginComp
    },
    
    

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
