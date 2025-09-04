<template>
  <div class="flex flex-col min-h-screen">
    <Navbar :show-cart="showCart" :secure-message="secureMessage" />

    <main class="flex-grow">
      <slot />
    </main>

    <Footer />
  </div>
</template>

<script setup lang="ts">
import Navbar from '@/components/organisms/Navbar.vue'
import Footer from '@/components/organisms/Footer.vue'

defineProps<{
  showUser?: boolean
  showCart?: boolean
  secureMessage?: boolean
}>()
</script>
