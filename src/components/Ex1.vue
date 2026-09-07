<script setup>
    import { ref } from 'vue'

    // Add code here
    // challenge: use array  
    const message = ref("Choose your favourite fruit:")
    const items = ["apple","orange","peach"]
</script>

<template>
    {{ message }} 
    <template v-for="i in items">
        <label for="fruit"><input type="radio" name="fruit" >{{ i }}</label> 
    </template>
    
    
    
</template>

<style scoped>
</style>
