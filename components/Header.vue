<script setup>
import {ref} from 'vue';
const isMenuOpen = ref(false);

const toggleMenu = () => {
    isMenuOpen.value = !isMenuOpen.value;
};

</script>


<template>
    <header>
        <div class="responsive-container">
            <div class="header-wrapper">
                <div class="header-logo">
                    <a href="/">
                        <img class="img-fluid" src="~/assets/images/everpeak-logo.png" alt="logo-image">
                    </a>
                </div>

                <div :class="{ 'show-menu': isMenuOpen }" class="navbar-user-link">
                    <ul class="d-flex m-0 p-0 align-items-center list-unstyled">
                        <li>
                            <a class="navbar-link" href="/apply">Apply</a>
                        </li>
                        <li>
                            <a class="navbar-link" href="/about">About</a>
                        </li>
                        <li>
                            <a class="navbar-link" href="/programs">Programs</a>
                        </li>
                        <li>
                            <a class="navbar-link" href="/#invest">Invest</a>
                        </li>
                        <li>
                            <a class="navbar-link" href="/blog">Blog</a>
                        </li>
                        <li>
                            <button class="common-button header-button">
                                GET STARTED
                            </button>
                        </li>
                    </ul>
                </div>
                <div @click="toggleMenu" class="hamburger-images">
                    <img v-if="!isMenuOpen" class="responsive-images hamburger-image" src="~/assets/images/hamburger.svg" alt="hamburger">
                    <img v-else class="responsive-images cross-image" src="~/assets/images/cross-image.svg" alt="cross-image">
                </div>
            </div>
        </div>
    </header>
</template>

<style scoped>

</style>