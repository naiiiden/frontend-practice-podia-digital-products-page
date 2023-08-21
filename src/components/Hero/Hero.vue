<script setup>
import SignupLink from '../SignupLink/SignupLink.vue';

const props = defineProps({
    headingPreText: String,
    heading1: String,
    heading2: String,
    paragraph: String,
    link: String,
    linkSecondary: String,
    img: String,
})
</script>

<template>
    <div class="hero-container">
        <div class="hero-text">
            <span class="hero-pre-heading">{{ headingPreText }}</span>
            <h1 v-if="heading1">{{ heading1 }}</h1>
            <h3 v-if="heading2">{{ heading2 }}</h3>
            <p>{{ paragraph }}</p>
            <SignupLink v-if='link' :linkText='link'/>
            <a v-if="linkSecondary" href="" class="hero-link-secondary">{{ linkSecondary }} <span>→</span></a>
        </div>
        <img :src="img" alt="">
    </div>
</template>

<style lang="scss" scoped>

</style>