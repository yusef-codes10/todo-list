<script setup></script>

<template>
  <nav>
    <h2>Todo-list</h2>
    <div class="icons">
      <i class="fa-solid fa-moon"></i>
      <i class="fa-regular fa-sun"></i>
    </div>
  </nav>
</template>

<style scoped>
nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: min(1rem, 10vw);
}

nav h2 {
  font-size: clamp(1.8rem, 3vw + 0.75rem, 2rem);
  color: var(--brand-color);
  transition:
    color 0.4s ease,
    text-shadow 0.4s ease;
}

nav h2:hover {
  color: var(--text-color);
  text-shadow:
    0 0 5px var(--brand-color),
    0 0 15px var(--brand-color),
    0 0 30px var(--brand-color);
}

nav i {
  color: var(--brand-color);
  font-size: clamp(1rem, 4vw, 1.5rem);
}
</style>
