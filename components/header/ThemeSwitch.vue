<template>
    <label class="switch">
        <input type="checkbox" id="toggleMode">
        <span class="slider"></span>
    </label>
</template>

<script lang="ts" setup>
if (process.client) {
    const toggleSwitch = document.getElementById('toggleMode') as HTMLInputElement;

    if (toggleSwitch) {
        toggleSwitch.addEventListener('change', () => {
            const isChecked = toggleSwitch.checked;
            document.body.classList.toggle('dark-mode', isChecked);
        });
    }
}
</script>

<style scoped>
.switch {
    position: relative;
    display: inline-block;
    width: 50px;
    height: 30px;
    margin: 0 3vw 0 14vw;
}

.switch input {
    opacity: 0;
    width: 0;
    height: 0;
}

.slider {
    position: absolute;
    cursor: pointer;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    border: 1px black solid;
    border-radius: 30px;
    transition: .4s;
}

.slider:before {
    position: absolute;
    content: "";
    height: 24px;
    width: 24px;
    right: 2px;
    bottom: 2px;
    background-color: black;
    border-radius: 50%;
    transition: .4s;
    background-image: url('/images/moon-solid-24.png');
    background-size: 18px;
    background-repeat: no-repeat;
    background-position: center;
}

input:checked + .slider {
    background-color: black;
}

input:checked + .slider:before {
    transform: translateX(-20px);
    background-image: url('/images/sun-solid-24.png');
    background-color: white;
}
</style>