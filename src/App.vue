<script setup>
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
import { useCounterStore } from './stores/counter'

const userStore = useCounterStore()
console.log(userStore.count)
</script>

<template>
  <RouterView />
</template>

<style lang="scss">
 body {
  header {
    background-color: green;
  }
 }

</style>
