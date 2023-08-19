<script setup>
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
            <span>{{ headingPreText }}</span>
            <h1 v-if="heading1">{{ heading1 }}</h1>
            <h2 v-if="heading2">{{ heading2 }}</h2>
            <p>{{ paragraph }}</p>
            <a v-if="link" href="">{{ link }}</a>
            <a v-if="linkSecondary" href="">{{ linkSecondary }} <span>→</span></a>
        </div>
        <img :src="img" alt="">
    </div>
</template>

<style lang="scss" scoped>

</style>