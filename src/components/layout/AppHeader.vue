<script setup lang="ts">
import { ref } from 'vue'
import { Menu, X } from '@lucide/vue'
import DesktopNav from './DesktopNav.vue'
import MobileNav from './MobileNav.vue'

const isActive = ref(false)
</script>

<template>
  <header class="w-full bg-white "
          :class="{ 'border-b border-gray-200': !isActive }"
  >
    <div
        class="h-16 md:h-20 max-w-360 mx-auto flex items-center justify-between bg-white px-6"
    >
      <RouterLink to="/">
        <img
            src="https://placehold.co/160x48"
            alt="Logo"
            class="h-12 w-40"
        >
      </RouterLink>

      <DesktopNav />

      <button
          class="md:hidden cursor-pointer"
          type="button"
          aria-label="Toggle navigation"
          @click="isActive = !isActive"
      >
        <X v-if="isActive" />
        <Menu v-else />
      </button>
    </div>

    <MobileNav
        :is-active="isActive"
        @close="isActive = false"
    />
  </header>
</template>