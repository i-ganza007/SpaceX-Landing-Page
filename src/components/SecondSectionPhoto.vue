<template>
    <section id="secondSection">
        <sectionAText :launch_text="launch_text" :starship="starship"/>
        <scrolldown/>
    </section>
</template>
<script setup>
import { ref } from 'vue';
import scrolldown from './components/scrolldown.vue';
import sectionAText from './components/Section-a-Text.vue';
const launch_text = ref('RECENT LAUNCH');
const starship = ref('NROL-126 MISSION');
</script>