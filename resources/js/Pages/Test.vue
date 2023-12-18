<template>
    <div>
        <Link href="/test">Test</Link>
        <Link href="/about">About</Link>
        <br>
        <h1>Test Page</h1>
        <p>This is a test page</p>
        <button @click.prevent="incrementHandler">+</button>
        {{ count }}
        <button @click.prevent="decrementHandler">-</button>
    </div>
</template>

<script setup>
    import { ref } from 'vue'
    import { Link } from '@inertiajs/vue3'

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