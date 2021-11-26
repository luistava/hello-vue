<template>
    <div>
        
        <button v-on:click="update">Update Title</button>
    </div>
</template>

<script>
export default {
    name:"ChildComponent",
    methods:{
        update(){
            this.$emit('ChangeTitle','Props has been passed')
        }
    }

}
</script>