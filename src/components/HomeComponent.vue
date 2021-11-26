
<template>
    <div class="home">
        <h1>Home Componet</h1>
        <UsersComponent/>
        <ProductsComponent/>
    </div>
</template>

<script>
import UsersComponent from './UsersComponent.vue'
import ProductsComponent from './ProductComponents.vue'
export default {
    name:"HomeComponent",
    components:{
        UsersComponent,
        ProductsComponent
    }
}
</script>

<style scoped>
.home{
    background-color: aquamarine;
    height: 500px;
}
</style>