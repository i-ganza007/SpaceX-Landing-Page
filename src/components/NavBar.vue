<template>
    <section class="nav-sect">
        <div class="nav-bar">
            <nav id="top-part" :class="{ 'hidden': isNavHidden }">
                <div class="logo-image">
                    <img src="../assets/logo.png" alt="logo" id="space-logo">
                </div>

                <div class="links">
                    <ul>
                        <li><a href="">FALCON 9</a></li>
                        <li><a href="">FALCON HEAVY</a></li>
                        <li><a href="">DRAGON</a></li>
                        <li><a href="">STARSHIP</a></li>
                        <li><a href="">HUMAN SPACEFLIGHT</a></li>
                        <li><a href="">RIDESHARE</a></li>
                        <li><a href="">STARSHIELD</a></li>
                        <li><a href="">STARLINK</a></li>
                    </ul>
                </div>

                <div class="side-piece">
                    <a href="">SHOP</a>
                    <BurgerMenu @toggle="toggleMenu" class="burger-menu-component"/>
                </div>
                
            </nav>
        </div>

        <sectionAText :launch_text=launch_text  :starship=starship />
        <scrolldown/>
    </section>
</template>

<script setup>
import { ref } from 'vue'
import sectionAText from '@/components/Section-a-Text.vue';
import scrolldown from '@/components/scrolldown.vue';
import BurgerMenu from '@/components/BurgerMenu.vue'  // Make sure this path is correct

const launch_text = ref('RECENT LAUNCH');
const starship = ref('STARSHIP\'S SIXTH FLIGHT TEST');

const isMenuOpen = ref(false)



const toggleMenu = () => {
    isMenuOpen.value = !isMenuOpen.value
}

</script>

