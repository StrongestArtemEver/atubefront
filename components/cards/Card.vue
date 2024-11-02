<template>
    <a class="card" href="#">
        <div class="card__image"></div>
        <div class="card__description">
            <slot />
        </div>
    </a>

</template>

<script lang="ts" setup>

</script>

<style scoped>
.card {
    cursor: pointer;
    height: 15em;
    display: flex;
    flex-direction: column;
    text-decoration: none;
    color: black;
}

.card__image {
    background-color: lightgrey;
    border-radius: 8px;
    width: 100%;
    height: 100%;
}

.card__description {
    padding-top: 4px;
    font-size: 1.3rem;
    width: 100%;
}
</style>