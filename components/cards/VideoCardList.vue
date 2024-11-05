<template>
  <div class="videos-card-list">
    <Card>Video description</Card>
    <Card>Video description</Card>
    <Card>Video description</Card>
    <Card>Video description</Card>
    <Card>Video description</Card>
  </div>
</template>

<script lang="ts" setup>
import Card from './Card.vue';

</script>

<style scoped>
.videos-card-list {
  display: flex;
  flex-direction: column;
  width: 100%;
  row-gap: 1em;
}

.videos-card-list > * {
  height: 10vw;
  max-height: 13em;
  font-size: 1.1rem;
}
</style>