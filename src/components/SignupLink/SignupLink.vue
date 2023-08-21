<script setup>
const props = defineProps({
    linkText: String,
})
</script>

<template>
    <a href="" class="sign-up-link">{{ linkText }}</a>
</template>

