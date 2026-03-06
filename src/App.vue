<!-- Vue3 Composition API -->
<script setup lang="ts">
import { ref } from 'vue';

const msg = ref('Hello');
const myStyle = { color: 'gray' };
const title = 'Hello Vue';
</script>

<template>
  <h1>{{ msg }}</h1>
  <input v-model="msg" />

  <h2 v-bind:style="myStyle">{{ title }}</h2>
  <h2 :style="myStyle">데이터 바인딩</h2>
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
