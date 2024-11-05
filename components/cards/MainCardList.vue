<template>
    <div class="card-list">
        <Card>WOW</Card>
        <Card>Gachi</Card>
        <Card>Muchi</Card>
        <Card>Video description</Card>
        <Card>Video description</Card>
        <Card>Video description</Card>
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

<style>
.card-list {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(23em, 1fr));
    column-gap: 2rem;
    row-gap: 1rem;
}

.card-list .card {
    height: 14em;
    font-size: 1.3rem;
}
</style>