<template>
    <div>
        <h1 class="vueStyle">Class and Style Bindings</h1>
        <h1 v-bind:style="{color:colorName}">Style Bindings</h1>
        <h1 v-bind:class="{display:show}">Class with object</h1>
    </div>
</template>

<script>
export default {
    name:"HomeComponent2",
    data(){ 
        return{
            colorName:'skyblue',
            show:true
        }
    }

}
</script>

<style scoped>
    .vueStyle{
        color: orange;
    }

    .display{
        background-color: peru;
        padding: 5px;
    }
</style>