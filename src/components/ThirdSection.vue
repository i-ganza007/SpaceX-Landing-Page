<template>
    <section id="thirdSection">
        <SectionAText :launch_text="launch_text" :starship="starship"/>
        <Scrolldown/>
    </section>
</template>
<script setup>
import { ref } from 'vue';
import Scrolldown from './components/scrolldown.vue';
import SectionAText from './components/section-a-text.vue';

const launch_text = ref('RECENT LAUNCH');
const starship = ref('STARLINK MISSION');
</script>