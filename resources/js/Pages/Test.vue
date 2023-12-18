<template>
    <div>
        <h1>Test Page</h1>
        <p>This is a test page</p>
        <button @click.prevent="incrementHandler">+</button>
        {{ count }}
        <button @click.prevent="decrementHandler">-</button>
    </div>
</template>

<script>
    import { ref } from 'vue'
    export default {
        name:'Test',
        setup(){
            const count = ref(0)

            function incrementHandler(){
                count.value++
            }
            function decrementHandler(){
                count.value--
            }
            return {
                count,
                incrementHandler,
                decrementHandler
            }
        }
    }
</script>

<style lang="scss" scoped>

</style>