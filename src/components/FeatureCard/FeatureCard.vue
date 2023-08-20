<script setup>
const props = defineProps({
    img: String,
    h3: String,
    paragraph: String,
})
</script>

<template>
    <div class="feature-card">
        <img :src=img alt=""/>
        <h3>{{ h3 }}</h3>
        <p>{{ paragraph }}</p>
    </div>
</template>
