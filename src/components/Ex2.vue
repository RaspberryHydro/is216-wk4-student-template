<script setup>
    import { ref } from 'vue'

    // Add code here
    const width = ref(200)
    const height = ref(200)
    const myImg = ref('/assets/me.png')

    const obj = ref({
        width: '200',
        height: '200',
        src: '/assets/me.png'
    })

</script>

<template>

 <img :src="myImg" :height="height" :width="width" />
 <img v-bind="obj"/>
</template>
