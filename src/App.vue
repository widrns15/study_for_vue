<!-- Vue3 Composition API -->
<script setup lang="ts">
import { ref } from 'vue';

const foods = ['apple', 'banana', 'mango'];
const favoriteFoods = [
  { id: 0, name: 'strawberry' },
  { id: 1, name: 'melon' },
];

const isOpen = ref(true);
const closeModal = () => {
  isOpen.value = false;
};
</script>

<template>
  <h1>반복문</h1>
  <ul>
    <li v-for="(food, i) in foods" :key="i">{{ i }}: {{ food }}</li>
    <li v-for="favoriteFood in favoriteFoods" :key="favoriteFood.id">
      {{ favoriteFood.id }}: {{ favoriteFood.name }}
    </li>
  </ul>

  <h1>조건부 랜더링</h1>
  <div class="modal" v-if="isOpen">
    <h2>Notice</h2>
    <p>50% off today</p>
    <button @click="closeModal">close</button>
  </div>
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
