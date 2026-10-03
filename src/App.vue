<script setup lang="ts">

import AppHeader from "@/components/layout/AppHeader.vue";
</script>

<template>
  <header>
    <AppHeader class="fixed left-0 top-0"/>
  </header>
  <main>
    <RouterView/>
  </main>
</template>

<style scoped></style>
