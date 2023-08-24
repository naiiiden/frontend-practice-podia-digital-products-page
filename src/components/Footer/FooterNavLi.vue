<script setup>
const props = defineProps({
    liName: String,
})
</script>

<template>
    <li>
        <button class="footer-mobile-btn">
            {{ liName }}
            <svg width="10" viewBox="0 0 10 6" fill="none">
                <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M1 1l4 4 4-4"></path>
            </svg>
        </button>
        <h3 class="footer-desktop-section-link">
            {{ liName }}
        </h3>
        <slot></slot>
    </li>
</template>
