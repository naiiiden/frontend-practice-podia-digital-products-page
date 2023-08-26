<script setup>
// ChatGPT
import { ref, defineEmits } from 'vue';

const props = defineProps({
  liName: String,
  ariaLabel: String,
});

const emits = defineEmits();

const isOpen = ref(false);

const toggleDropdown = () => {
  isOpen.value = !isOpen.value;
  emits('toggleDropdown', props.liName);
};
</script>

<template>
    <li>
        <button class="footer-mobile-btn" @click="toggleDropdown"  aria-live="polite" :aria-label=ariaLabel>
            {{ liName }}
            <svg width="10" viewBox="0 0 10 6" fill="none" :class="{ rotate: isOpen }">
                <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M1 1l4 4 4-4"></path>
            </svg>
        </button>
        <h3 class="footer-desktop-section-link">
            {{ liName }}
        </h3>
        <slot></slot>
    </li>
</template>
