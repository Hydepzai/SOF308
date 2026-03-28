<template>
    <div>
        <h1>Caculator 18-Trương Tấn Gia Hy</h1>
        <h3>count {{ count }}</h3>
        <button @click="increment">+</button>
        <button @click="decrement">-</button>
        <button @click="reset">reset</button>

    </div>
    </template>
    <script setup>
import { ref } from 'vue'
const count = ref(0)
const increment = () => count.value++
const decrement = () => count.value--
const reset = () => (count.value = 0)
</script>