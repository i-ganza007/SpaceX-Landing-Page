<template>
    <section id="fourthSection">
        <SectionAText :launch_text="launch_text" :starship="starship"/>
        <scrolldown/>
    </section>
</template>
<script setup>
import { ref } from 'vue';
import SectionAText from '@/components/section-a-text.vue';
import scrolldown from '@/components/scrolldown.vue';
const launch_text = ref('RECENT LAUNCH')
const starship = ref('STARLINK MISSION')
</script>