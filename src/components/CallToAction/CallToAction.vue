<script setup>
import SignupLink from '../SignupLink/SignupLink.vue';

const props = defineProps({
    h2: String,
    paragraph: String,
    linkText: String,
})
</script>

<template>
    <section class="cta-container">
        <h2 v-if="h2">{{ h2 }}</h2>
        <p>{{ paragraph }}</p>
        <SignupLink v-if='linkText' :linkText='linkText'/>
    </section>
</template>

