<template>
  <div class="category-list">
    <Category>Music</Category>
    <Category>Podcasts</Category>
    <Category>Cats</Category>
  </div>
</template>

<script lang="ts" setup>
import Category from './Category.vue';

</script>

<style scoped>
.category-list {
    margin: 1.5rem 0 1rem 0;
    display: flex;
    gap: 1rem;
}
</style>