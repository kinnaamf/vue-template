<script setup lang="ts">

import AppHeader from "@/components/layout/AppHeader.vue";
</script>

<template>
  <header>
    <AppHeader class="sticky left-0 top-0"/>
  </header>
  <main class="max-w-[1440px] mx-auto">
    <RouterView/>
  </main>
</template>

<style scoped></style>
