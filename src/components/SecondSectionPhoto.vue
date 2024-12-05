<template>
    <section id="secondSection">
        <sectionAText :launch_text="launch_text" :starship="starship"/>
        <scrolldown/>
    </section>
</template>
<script setup>
import { ref } from 'vue';
import scrolldown from './scrolldown.vue';
import sectionAText from './section-a-text.vue';
const launch_text = ref('RECENT LAUNCH');
const starship = ref('NROL-126 MISSION');
</script>