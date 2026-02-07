<script setup>
import { ref } from 'vue'

// const todo = ref('')
const inputTodo = ref('')

// const check = () => {
//   todo.value = `hello ${inputTodo.value}`
// }

const todos = ref([])

const addTask = () => {
  // here we add a task to the array
  if (inputTodo.value.trim() === '') return
  todos.value.push(inputTodo.value)
  inputTodo.value = ''
}

const removeTodo = () => {
  // here is the logic for removing an array
}
</script>

<template>
  <div class="todo-container">
    <div class="user-input">
      <input type="text" v-model="inputTodo" />
      <button @click="addTask">Add</button>
    </div>
    <!-- <div class="greet-user">
      <h1>{{ todo }}</h1>
    </div> -->
    <div class="to-do-list">
      <ul>
        <li v-for="todo in todos" :key="todo">
          <span>{{ todo }}</span>
          <button @click="removeTodo">x</button>
        </li>
      </ul>
    </div>
  </div>
</template>

<style scoped></style>
