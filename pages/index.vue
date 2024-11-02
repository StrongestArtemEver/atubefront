<template>
  <div>
    <Header></Header>
    <Main></Main>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  name: 'IndexPage',
})
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Montserrat:ital,wght@0,100..900;1,100..900&display=swap');

* {
  padding: 0;
  margin: 0;
  font-family: "Monsterrat", sans-serif;
  user-select: none;
}

div {
  width: 75vw;
  margin: 0 auto;
}

button {
  background-color: black;
  color: white;
  border: 0;
  letter-spacing: .8px;
  cursor: pointer;
}
</style>
