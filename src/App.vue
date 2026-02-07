<script setup>
import { ref } from 'vue'

const todo = ref('')
const inputTodo = ref('')

const check = () => {
  todo.value = `hello ${inputTodo.value}`
}
</script>

<template>
  <div class="todo-container">
    <div class="user-input">
      <input type="text" v-model="inputTodo" />
      <button @click="check">Add</button>
    </div>
    <div class="greet-user">
      <h1>{{ todo }}</h1>
    </div>
  </div>
</template>

<style scoped></style>
