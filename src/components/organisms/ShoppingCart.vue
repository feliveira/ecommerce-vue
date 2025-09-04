<template>
  <button
    @click="isVisible = true"
    aria-label="Abrir carrinho"
    class="relative p-3 w-12 h-12 flex items-center justify-center bg-gradient-to-br from-blue-600 to-blue-700 hover:from-blue-700 hover:to-blue-800 rounded-full transition-all duration-200 transform hover:scale-105 shadow-lg border border-blue-400/30"
  >
    <i class="pi pi-shopping-cart text-lg"></i>
  </button>

  <Drawer
    v-model:visible="isVisible"
    header="Carrinho de Compras"
    position="right"
    class="w-full md:w-80 lg:w-96 bg-white"
  >
    <template #header>
      <div class="flex items-center gap-3">
        <h2 class="text-xl font-bold text-gray-900">Meu carrinho</h2>
        <span class="bg-gray-200 text-gray-700 px-2 py-1 rounded-full text-xs">
          {{ cartItems.length }}
        </span>
      </div>
    </template>
    <div class="p-4">
      <p class="text-gray-700 mb-4">Seu carrinho está vazio no momento.</p>
    </div>
    <template #footer>
      <div class="border-t border-gray-100 p-6 bg-gray-50">
        <!-- Totals -->
        <div class="space-y-3 mb-6">
          <div class="flex justify-between text-gray-600">
            <span>Subtotal</span>
            <span>R$ {{ subtotal.toFixed(2) }}</span>
          </div>
        </div>

        <!-- Checkout Button -->
        <button
          class="w-full bg-gradient-to-br from-blue-600 to-blue-700 hover:from-blue-700 hover:to-blue-800 text-white py-4 rounded-xl font-semibold text-lg transition-all duration-200 transform hover:scale-[1.02] active:scale-[0.98] shadow-lg"
        >
          Finalizar Compra
        </button>

        <!-- Continue Shopping -->
        <button
          @click="isVisible = false"
          class="w-full mt-3 text-gray-600 hover:text-gray-900 py-2 font-medium transition-colors duration-200"
        >
          Continuar Comprando
        </button>
      </div>
    </template>
  </Drawer>
</template>

<script setup lang="ts">
import Drawer from 'primevue/drawer'
import { computed, ref } from 'vue'

const isVisible = ref(false)

interface CartItem {
  id: number
  title: string
  image: string
  price: number
  category: string
  quantity: number
}

const cartItems = ref<CartItem[]>([])

const subtotal = computed(() => {
  return cartItems.value.reduce(
    (sum, item) => sum + item.price * item.quantity,
    0
  )
})
</script>
