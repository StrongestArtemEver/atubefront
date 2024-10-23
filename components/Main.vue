<template>
  <main>
    <a class="card" href="#">
      <div class="card__image"></div>
      <div class="card__description">
        <p>Yes</p>
      </div>
    </a>
    <a class="card" href="#">
      <div class="card__image"></div>
      <div class="card__description">
        <p>Brawl Stars</p>
      </div>
    </a>
    <a class="card" href="#">
      <div class="card__image"></div>
      <div class="card__description">
        <p>WOT</p>
      </div>
    </a>
  </main>
</template>

<script lang="ts" setup>

</script>

<style scoped>
main {
  width: 75vw;
  margin: 0 auto;
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(18em, 20em));
  /* justify-content: space-between; */
  gap: 1rem;
}

.card {
  cursor: pointer;
  /* width: clamp(8em, 15em, 1fr); */
  height: 14em;
  display: flex;
  flex-direction: column;
  text-decoration: none;
  color: black;
}

.card__image {
  background-color: lightgrey;
  width: 100%;
  height: 100%;
  border-radius: 8px;
}

.card__description {
  padding: 6px 4px 0 4px;
  font-size: 1.3rem;
}
</style>