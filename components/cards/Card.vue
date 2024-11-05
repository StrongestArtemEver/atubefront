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
    height: 12rem;
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
    padding: 6px 4px 0 4px;
    width: 100%;
}
</style>