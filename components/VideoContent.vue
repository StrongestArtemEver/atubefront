<template>
  <main>
    <VideoDetails></VideoDetails>
    <VideoCardList></VideoCardList>
  </main>
</template>

<script lang="ts" setup>
import VideoCardList from './cards/VideoCardList.vue';
import VideoDetails from './video details/VideoDetails.vue';


</script>

<style scoped>
main {
  display: grid;
  grid-template-columns: 1fr 15vw;
  gap: 5em;
  margin-top: 2rem;
}
</style>