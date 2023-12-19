<template>
    <div>
     
        <br>
        <h1>Test Page</h1>
        <p>This is a test page</p>
        <button @click.prevent="incrementHandler">+</button>
        {{ count }}
        <button @click.prevent="decrementHandler">-</button>
        <Footer />
    </div>
</template>

<script setup>
import Footer from './Footer.vue'
    import { ref } from 'vue'
  

    const count = ref(0)

    function incrementHandler(){
        count.value++
    }
    function decrementHandler(){
        count.value--
    }
         
    
</script>

<style lang="scss" scoped>

</style>