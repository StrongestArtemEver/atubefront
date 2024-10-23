<template>
  <header>
    <h1>Atube</h1>
    <Search></Search>
  </header>
</template>

<script lang="ts" setup>
import Search from './Search.vue';


</script>

<style scoped>
header {
  width: 75vw;
  margin: 32px auto 1em auto;
  border-bottom: .3em lightgrey solid;
  border-radius: 2px;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

h1 {
  font-size: 3rem;
  font-weight: 400;
  padding: 0 4rem;
}
</style>