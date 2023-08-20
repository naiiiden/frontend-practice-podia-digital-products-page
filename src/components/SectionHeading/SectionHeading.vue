<script setup>
const props = defineProps({
    heading: String,
    paragraph: String,
})
</script>

<template>
    <div class="section-heading">
        <h2>{{ heading }}</h2>
        <p>{{ paragraph }}</p>
    </div>
</template>

