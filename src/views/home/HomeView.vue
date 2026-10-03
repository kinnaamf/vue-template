<script setup lang="ts">

import HeroSection from "@/views/home/sections/HeroSection.vue";
import StatsBlock from "@/components/home/StatsBlock.vue";
import RankingSection from "@/views/home/sections/RankingSection.vue";
</script>

<template>
  <div class="flex flex-col gap-16">
    <HeroSection/>
    <StatsBlock/>
    <RankingSection/>
  </div>
</template>

<style scoped>

</style>