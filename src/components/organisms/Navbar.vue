<template>
  <nav
    class="w-full bg-gradient-to-r from-slate-900 via-blue-900 to-slate-900 text-white shadow-2xl border-b border-blue-500/20 sticky top-0 z-50 backdrop-blur-sm"
  >
    <div class="max-w-7xl mx-auto px-6 py-4">
      <div class="flex justify-between items-center">
        <!-- Brand -->
        <div class="flex items-center gap-3">
          <div
            class="w-10 h-10 bg-gradient-to-br from-blue-400 to-sky-500 rounded-xl flex items-center justify-center shadow-lg"
          >
            <i class="pi pi-shopping-bag text-white text-lg"></i>
          </div>
          <div>
            <span
              class="text-2xl font-bold bg-gradient-to-r from-blue-300 via-zinc-100 to-zinc-300 bg-clip-text text-transparent"
            >
              FakeStore
            </span>
            <p class="text-xs text-zinc-50 -mt-1">Premium Collection</p>
          </div>
        </div>

        <!-- Right side -->
        <div class="flex items-center gap-4">
          <!-- Cart button -->
          <div v-if="showCart" class="relative">
            <button
              aria-label="Abrir carrinho"
              class="relative p-3 w-12 h-12 flex items-center justify-center bg-gradient-to-br from-blue-600 to-blue-700 hover:from-blue-700 hover:to-blue-800 rounded-full transition-all duration-200 transform hover:scale-105 shadow-lg border border-blue-400/30"
            >
              <i class="pi pi-shopping-cart text-lg"></i>
            </button>
          </div>

          <!-- Safe purchase message -->
          <div
            v-if="secureMessage"
            class="hidden lg:flex items-center gap-2 bg-emerald-500/20 backdrop-blur-sm px-3 py-2 rounded-full border border-emerald-400/30"
          >
            <i class="pi pi-shield-check text-emerald-400 text-sm"></i>
            <span class="text-emerald-300 font-medium text-sm">
              Compra 100% Segura
            </span>
          </div>
        </div>
      </div>
    </div>
  </nav>
</template>

<script setup lang="ts">
defineProps<{
  showCart?: boolean
  secureMessage?: boolean
}>()
</script>
