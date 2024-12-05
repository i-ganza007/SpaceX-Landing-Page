<template>
    <div class="sectiona-container">
        <h3 id="launch-text">{{ launch_text }}</h3>
        <p id="starship-text">{{starship}}</p>
        <button id="section-a-rewatch">{{ button }}</button>
    </div>
</template>

<script setup>
import { ref } from 'vue';
import {defineProps} from 'vue';
const props = defineProps({
    launch_text:{
        type:String,
        default: '',
        required:true
    },
    starship:{
        type:String,
        required:true
    },
    button:{
        type:String,
        default:'REWATCH'
    }
})
</script>