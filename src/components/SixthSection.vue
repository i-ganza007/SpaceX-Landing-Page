<template>
    <section id="sixth">
        <sectionAText  :starship="starship" :button="button"/>
        <scrolldown/>
    </section>
</template>
<script setup>
import { ref } from 'vue';
import scrolldown from './scrolldown.vue';
import sectionAText from './Section-a-Text.vue';
const button = ref('LEARN MORE')
const starship = ref('TO MAKE LIFE MULTIPLANETARY ')
</script>