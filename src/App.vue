<!-- Vue3 Composition API -->
<script setup lang="ts">
const title = '너의 이름은';
const year = 2016;
const category = '판타지';
</script>

<template>
  <h1>{{ title }}</h1>
  <p>개봉: {{ year }}</p>
  <p>장르: {{ category }}</p>
</template>

<!-- Vue2 Options API -->
<!-- <script lang="ts">
export default {
  name: 'App',
  data() {
    return {
      title: '노량',
      year: 2023,
      category: '액션',
    };
  },
};
</script>

<template>
  <h1>{{ title }}</h1>
  <p>개봉: {{ year }}</p>
  <p>장르: {{ category }}</p>
</template> -->

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
