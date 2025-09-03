<template>
  <footer
    class="relative bg-gradient-to-br from-slate-900 via-blue-900 to-slate-900 text-white py-20 px-4 md:px-16 overflow-hidden"
  >
    <div class="max-w-7xl mx-auto relative z-10">
      <div class="relative mb-12">
        <hr class="border-blue-400/20" />
      </div>

      <!-- Main footer content -->
      <div class="grid grid-cols-1 md:grid-cols-4 gap-12 mb-16">
        <!-- Brand -->
        <div class="md:col-span-2">
          <div class="flex items-center gap-3 mb-6">
            <div
              class="w-10 h-10 bg-gradient-to-br from-blue-400 to-sky-500 rounded-xl flex items-center justify-center shadow-lg"
              style="animation-delay: 1s; animation-duration: 2s"
            >
              <i class="pi pi-shopping-bag text-white text-xl"></i>
            </div>
            <div>
              <h3
                class="text-2xl font-bold bg-gradient-to-r from-blue-300 via-zinc-100 to-zinc-300 bg-clip-text text-transparent"
              >
                FakeStore
              </h3>
              <p class="text-xs text-zinc-50 -mt-1">Premium Collection</p>
            </div>
          </div>
          <p class="text-blue-100 mb-6 leading-relaxed max-w-md">
            Sua loja online de confiança com os melhores produtos e preços
            imbatíveis. Qualidade garantida e entrega rápida para todo o Brasil.
          </p>

          <!-- Newsletter signup -->
          <div class="relative">
            <div
              class="flex bg-white/10 backdrop-blur-sm rounded-full border border-blue-400/30 overflow-hidden hover:border-blue-400/50 transition-all duration-300 group"
            >
              <input
                type="email"
                placeholder="Seu e-mail para ofertas exclusivas"
                class="bg-transparent text-white placeholder-blue-200 px-6 py-3 flex-1 focus:outline-none"
              />
              <button
                class="bg-gradient-to-r from-blue-600 to-blue-700 hover:from-blue-700 hover:to-blue-800 px-6 py-3 transition-all duration-200 group-hover:scale-105"
              >
                <i class="pi pi-send text-white"></i>
              </button>
            </div>
          </div>
        </div>

        <!-- Navigation Links -->
        <div class="space-y-6">
          <h4 class="font-semibold text-lg text-white relative">
            Navegação
            <div
              class="absolute -bottom-1 left-0 w-8 h-0.5 bg-gradient-to-r from-blue-400 to-sky-400"
            ></div>
          </h4>
          <ul class="space-y-4">
            <li>
              <a
                href="#"
                class="text-blue-100 hover:text-white transition-all duration-200 flex items-center gap-2 group"
              >
                <i
                  class="pi pi-home text-sm group-hover:scale-110 transition-transform"
                ></i>
                <span class="group-hover:translate-x-1 transition-transform"
                  >Início</span
                >
              </a>
            </li>
            <li>
              <a
                href="#"
                class="text-blue-100 hover:text-white transition-all duration-200 flex items-center gap-2 group"
              >
                <i
                  class="pi pi-box text-sm group-hover:scale-110 transition-transform"
                ></i>
                <span class="group-hover:translate-x-1 transition-transform"
                  >Produtos</span
                >
              </a>
            </li>
            <li>
              <a
                href="#"
                class="text-blue-100 hover:text-white transition-all duration-200 flex items-center gap-2 group"
              >
                <i
                  class="pi pi-tags text-sm group-hover:scale-110 transition-transform"
                ></i>
                <span class="group-hover:translate-x-1 transition-transform"
                  >Categorias</span
                >
              </a>
            </li>
            <li>
              <a
                href="#"
                class="text-blue-100 hover:text-white transition-all duration-200 flex items-center gap-2 group"
              >
                <i
                  class="pi pi-percentage text-sm group-hover:scale-110 transition-transform"
                ></i>
                <span class="group-hover:translate-x-1 transition-transform"
                  >Ofertas</span
                >
              </a>
            </li>
            <li>
              <a
                href="#"
                class="text-blue-100 hover:text-white transition-all duration-200 flex items-center gap-2 group"
              >
                <i
                  class="pi pi-phone text-sm group-hover:scale-110 transition-transform"
                ></i>
                <span class="group-hover:translate-x-1 transition-transform"
                  >Contato</span
                >
              </a>
            </li>
          </ul>
        </div>

        <!-- Support Links -->
        <div class="space-y-6">
          <h4 class="font-semibold text-lg text-white relative">
            Suporte
            <div
              class="absolute -bottom-1 left-0 w-8 h-0.5 bg-gradient-to-r from-blue-400 to-sky-400"
            ></div>
          </h4>
          <ul class="space-y-4">
            <li>
              <a
                href="#"
                class="text-blue-100 hover:text-white transition-all duration-200 flex items-center gap-2 group"
              >
                <i
                  class="pi pi-shield text-sm group-hover:scale-110 transition-transform"
                ></i>
                <span class="group-hover:translate-x-1 transition-transform"
                  >Política de Privacidade</span
                >
              </a>
            </li>
            <li>
              <a
                href="#"
                class="text-blue-100 hover:text-white transition-all duration-200 flex items-center gap-2 group"
              >
                <i
                  class="pi pi-file text-sm group-hover:scale-110 transition-transform"
                ></i>
                <span class="group-hover:translate-x-1 transition-transform"
                  >Termos de Uso</span
                >
              </a>
            </li>
            <li>
              <a
                href="#"
                class="text-blue-100 hover:text-white transition-all duration-200 flex items-center gap-2 group"
              >
                <i
                  class="pi pi-refresh text-sm group-hover:scale-110 transition-transform"
                ></i>
                <span class="group-hover:translate-x-1 transition-transform"
                  >Trocas e Devoluções</span
                >
              </a>
            </li>
            <li>
              <a
                href="#"
                class="text-blue-100 hover:text-white transition-all duration-200 flex items-center gap-2 group"
              >
                <i
                  class="pi pi-truck text-sm group-hover:scale-110 transition-transform"
                ></i>
                <span class="group-hover:translate-x-1 transition-transform"
                  >Entrega</span
                >
              </a>
            </li>
            <li>
              <a
                href="#"
                class="text-blue-100 hover:text-white transition-all duration-200 flex items-center gap-2 group"
              >
                <i
                  class="pi pi-question-circle text-sm group-hover:scale-110 transition-transform"
                ></i>
                <span class="group-hover:translate-x-1 transition-transform"
                  >FAQ</span
                >
              </a>
            </li>
          </ul>
        </div>
      </div>

      <div class="relative mb-8">
        <hr class="border-blue-400/20" />
      </div>

      <!-- Bottom section -->
      <div class="flex flex-col md:flex-row items-center justify-between">
        <div class="text-center md:text-left mb-6 md:mb-0">
          <p class="text-blue-100 font-medium">
            © 2025 FakeStore Premium Collection
          </p>
          <p class="text-blue-300 text-sm mt-1">Feito com ❤️</p>
        </div>

        <div class="flex items-center gap-4">
          <div class="flex gap-3">
            <a
              target="_blank"
              rel="noopener"
              href="https://github.com/feliveira/ecommerce-vue"
              class="group relative"
            >
              <div
                class="w-10 h-10 bg-gradient-to-br from-gray-800 to-gray-900 rounded-full border flex items-center justify-center transition-all duration-200 group-hover:scale-110 group-hover:shadow-lg group-hover:shadow-gray-500/25"
              >
                <i
                  class="pi pi-github text-white text-sm group-hover:animate-pulse"
                ></i>
              </div>
            </a>
          </div>
        </div>
      </div>

      <!-- Floating particles effect -->
      <div class="absolute top-0 left-0 w-full h-full pointer-events-none">
        <div
          class="absolute top-1/4 left-1/4 w-2 h-2 bg-blue-400/30 rounded-full animate-ping"
          style="animation-delay: 0s; animation-duration: 3s"
        ></div>
        <div
          class="absolute top-3/4 right-1/4 w-1 h-1 bg-blue-400/30 rounded-full animate-ping"
          style="animation-delay: 1s; animation-duration: 4s"
        ></div>
        <div
          class="absolute top-1/2 right-1/3 w-1.5 h-1.5 bg-blue-300/20 rounded-full animate-ping"
          style="animation-delay: 2s; animation-duration: 5s"
        ></div>
      </div>
    </div>
  </footer>
</template>
