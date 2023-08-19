<script setup>
import Header from './components/header/Header.vue';
import { openDropdown } from './components/header/openDropdown';
import Hero from './components/hero/Hero.vue';
</script>

<template>
  <Header/>
  <div @click="openDropdown = !openDropdown">
    <main>
      <Hero/>
    </main>
  </div>
</template>