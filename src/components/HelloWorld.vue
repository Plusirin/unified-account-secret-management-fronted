<script setup>
import {ref} from 'vue'

defineProps({
    msg: String
})

let count = ref(0)

let btn = () => {
    count.value++
}


</script>

<template>
    <h1>{{ msg }}</h1>

    <button type="button" @click="btn">count is: {{ count }}</button>

</template>

<style scoped>
h1 {
    color: #42b983;
}
</style>
