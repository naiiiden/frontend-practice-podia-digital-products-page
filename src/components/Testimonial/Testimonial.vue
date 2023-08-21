<script setup>
const props = defineProps({
    blockquote: String,
    figcaption: String,
})
</script>

<template>
    <figure>
        <img src="src/assets/stars.png" alt="">
        <blockquote>
            {{ blockquote }}
        </blockquote>
        <figcaption>
            {{ figcaption }}
        </figcaption>
    </figure>
</template>

