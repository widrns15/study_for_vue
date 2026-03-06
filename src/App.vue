<!-- Vue3 Composition API -->
<script setup lang="ts">
import { ref } from 'vue';
let count = ref(0);
const increment = () => {
  count.value++;
};
const decrement = () => {
  count.value--;
};
</script>

<template>
  <p>Count: {{ count }}</p>
  <button @click="increment">Count++</button>
  <button v-on:click="decrement" style="margin-left: 20px">Count--</button>
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
