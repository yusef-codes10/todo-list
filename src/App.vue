<script setup>
import { ref } from 'vue'

const todo = ref('Jake')

const check = () => {}
</script>

<template>
  <div class="todo-container">
    <div class="user-input">
      <input type="text" v-model="todo" />
      <button @click="check">Add</button>
    </div>
    <div class="greet-user">
      <h1>{{ todo }}</h1>
    </div>
  </div>
</template>

<style scoped></style>
