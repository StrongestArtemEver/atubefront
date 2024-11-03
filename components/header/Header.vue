<template>
    <header>
        <h1>Atube</h1>
        <ThemeSwitch></ThemeSwitch>
        <Search></Search>
    </header>
</template>

<script lang="ts" setup>
import Search from './Search.vue';
import ThemeSwitch from './ThemeSwitch.vue'


</script>

<style scoped>
header {
    margin: 1em 0 .6em;
    display: flex;
    align-items: center;
    position: relative;
}

header::before {
    width: 100%;
    height: .4em;
    background-color: black;
    border-radius: 12px;
    content: '';
    position: absolute;
    bottom: -.6em;
    left: 0;
}

h1 {
    font-size: 3rem;
    font-weight: 400;
    padding: 0 4rem;
}

</style>