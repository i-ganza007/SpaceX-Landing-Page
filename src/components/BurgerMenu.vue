<template>
    <div class="burger-menu" @click="toggleMenu" :class="{ 'active': isOpen }">
        <div class="burger-bar"></div>
        <div class="burger-bar"></div>
        <div class="burger-bar"></div>
    </div>
</template>

<script setup>
import { ref } from 'vue';

const isOpen = ref(false);
const emit = defineEmits(['toggle']);

const toggleMenu = () => {
    isOpen.value = !isOpen.value;
    emit('toggle');
}
</script>