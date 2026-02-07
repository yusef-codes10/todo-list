<script setup>
import { ref } from 'vue'

const todo = ref('Jake')
</script>

<template>
  <div class="todo-container">
    <div class="user-input">
      <input type="text" v-model="todo" />
      <button>Add</button>
    </div>
  </div>
</template>

<style scoped></style>
