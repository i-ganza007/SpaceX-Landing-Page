<template>
    <section id="fifth">
        <sectionAText :starship="starship" :button="button"/>
        <scrolldown/>
    </section>
</template>
<script setup>
import scrolldown from './components/scrolldown.vue';
import { ref } from 'vue';
import sectionAText from './components/Section-a-Text.vue';
const button = ref('LEARN MORE')
const starship = ref("ADVANCING HUMAN SPACEFLIGHT") 
</script>