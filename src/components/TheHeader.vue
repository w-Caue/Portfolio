<template>
  <header class="relative min-h-screen">

    <nav class="fixed top-0 left-0 z-50 w-full flex justify-center items-center px-5 py-4">
      <div
        class="flex items-center gap-8 px-6 py-3 bg-white/80 backdrop-blur-md border border-gray-100 shadow-lg rounded-full">

        <a href="#home" class="hidden sm:block text-[#2c3e50] font-bold uppercase tracking-wide">
          Cauê<span class="text-[#79BFFA]">.</span>
        </a>

        <ul class="hidden sm:flex items-center gap-6 uppercase font-semi text-sm">
          <li>
            <a href="#home" class="text-[#2c3e50] hover:text-[#79BFFA] transition-colors">
              Início
            </a>
          </li>

          <li>
            <a href="#about" class="text-[#2c3e50] hover:text-[#79BFFA] transition-colors">
              Sobre
            </a>
          </li>

          <li>
            <a href="#skills" class="text-[#2c3e50] hover:text-[#79BFFA] transition-colors">
              Skills
            </a>
          </li>

          <li>
            <a href="#project" class="text-[#2c3e50] hover:text-[#79BFFA] transition-colors">
              Projetos
            </a>
          </li>

          <li>
            <a href="#contact" class="text-[#2c3e50] hover:text-[#79BFFA] transition-colors">
              Contato
            </a>
          </li>
        </ul>

        <button @click="menuNav = !menuNav"
          class="sm:hidden text-[#2c3e50] cursor-pointer hover:scale-95 transition-transform" aria-label="Abrir menu">
          <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none"
            stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
            <path d="M4 5h16" />
            <path d="M4 12h16" />
            <path d="M4 19h16" />
          </svg>
        </button>
      </div>
    </nav>

    <Transition name="menu">
      <div v-if="menuNav" class="fixed inset-0 z-[60] bg-white sm:hidden">
        <div class="flex flex-col h-full p-6">

          <div class="flex items-center justify-between">
            <a href="#home" @click="closeMenu" class="text-xl text-[#2c3e50] font-bold uppercase">
              Cauê<span class="text-[#79BFFA]">.</span>
            </a>

            <button @click="closeMenu" class="text-[#2c3e50] cursor-pointer hover:rotate-90 transition-transform"
              aria-label="Fechar menu">
              <svg xmlns="http://www.w3.org/2000/svg" width="28" height="28" viewBox="0 0 24 24" fill="none"
                stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                <path d="M18 6 6 18" />
                <path d="m6 6 12 12" />
              </svg>
            </button>
          </div>

          <div class="h-px bg-gray-100 my-8"></div>

          <ul class="flex flex-col gap-6 text-lg font-bold uppercase">
            <li>
              <a href="#home" @click="closeMenu" class="text-[#2c3e50] hover:text-[#79BFFA] transition-colors">
                Início
              </a>
            </li>

            <li>
              <a href="#about" @click="closeMenu" class="text-[#2c3e50] hover:text-[#79BFFA] transition-colors">
                Sobre
              </a>
            </li>

            <li>
              <a href="#skills" @click="closeMenu" class="text-[#2c3e50] hover:text-[#79BFFA] transition-colors">
                Skills
              </a>
            </li>

            <li>
              <a href="#project" @click="closeMenu" class="text-[#2c3e50] hover:text-[#79BFFA] transition-colors">
                Projetos
              </a>
            </li>

            <li>
              <a href="#contact" @click="closeMenu" class="text-[#2c3e50] hover:text-[#79BFFA] transition-colors">
                Contato
              </a>
            </li>
          </ul>

          <div class="mt-auto">
            <p class="text-xs uppercase text-gray-400">
              Desenvolvedor Back-end Java
            </p>

            <div class="h-1 w-12 bg-[#79BFFA] rounded-full mt-2"></div>
          </div>
        </div>
      </div>
    </Transition>

    <section id="home" class="container mx-auto min-h-screen grid lg:grid-cols-2 items-center gap-12 px-5 pt-28 pb-16">

      <div class="text-start space-y-8">
        <div class="space-y-3">
          <span class="inline-flex items-center gap-2 text-xs uppercase tracking-widest text-[#79BFFA] font-bold">
            <span class="w-2 h-2 bg-[#79BFFA] rounded-full"></span>
            Olá, me chamo
          </span>

          <h1 class="text-4xl sm:text-6xl lg:text-7xl text-[#2c3e50] uppercase font-bold leading-tight">
            Cauê Sousa<span class="text-[#79BFFA]">.</span>
          </h1>

          <h2 class="text-lg sm:text-2xl text-[#2c3e50] font-bold uppercase">
            Desenvolvedor
            <span class="text-[#79BFFA]">Back-end Java</span>
          </h2>

          <div class="flex flex-wrap gap-2 pt-2">
            <span
              class="text-xs uppercase font-semibold text-[#2c3e50] border border-gray-200 px-3 py-1.5 rounded-full">
              Java
            </span>

            <span
              class="text-xs uppercase font-semibold text-[#2c3e50] border border-gray-200 px-3 py-1.5 rounded-full">
              Spring Boot
            </span>

            <span
              class="text-xs uppercase font-semibold text-[#2c3e50] border border-gray-200 px-3 py-1.5 rounded-full">
              REST API
            </span>
          </div>
        </div>

        <p class="max-w-xl text-sm sm:text-base leading-relaxed text-gray-600">
          Desenvolvedor focado na construção de APIs REST e aplicações web
          utilizando Java e Spring Boot, com experiência em desenvolvimento
          Full Stack e tecnologias como PHP, Laravel e Vue.js.
        </p>

        <div class="flex flex-wrap items-center gap-3">
          <button @click="visualizarCurriculo"
            class="group flex items-center gap-2 text-white text-sm uppercase font-bold bg-[#2c3e50] py-3 px-6 rounded-full cursor-pointer hover:bg-[#79BFFA] hover:text-[#2c3e50] transition-all">
            <svg xmlns="http://www.w3.org/2000/svg" width="18" height="18" viewBox="0 0 24 24" fill="none"
              stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
              <path d="M12 15V3" />
              <path d="m7 10 5 5 5-5" />
              <path d="M5 21h14" />
            </svg>
            Download CV
          </button>

          <a href="https://github.com/w-Caue" target="_blank" rel="noopener noreferrer"
            class="flex items-center gap-2 text-[#2c3e50] text-sm uppercase font-bold border border-gray-200 py-3 px-5 rounded-full hover:border-[#79BFFA] hover:text-[#79BFFA] transition-all">
            GitHub
          </a>

          <a href="https://www.linkedin.com/in/cauesousadev/" target="_blank" rel="noopener noreferrer"
            class="flex items-center gap-2 text-[#2c3e50] text-sm uppercase font-bold border border-gray-200 py-3 px-5 rounded-full hover:border-[#79BFFA] hover:text-[#79BFFA] transition-all">
            LinkedIn
          </a>
        </div>
      </div>

      <div class="relative flex justify-center lg:justify-end">
        <div class="absolute w-64 h-64 sm:w-80 sm:h-80 bg-[#79BFFA]/20 rounded-full blur-3xl"></div>

        <div class="relative">
          <div class="absolute -inset-3 border-2 border-[#79BFFA]/40 rounded-full"></div>

          <img class="relative w-64 h-64 sm:w-96 sm:h-96 object-cover rounded-full border-8 border-white shadow-2xl"
            src="../assets/img/ft-caue.png" alt="Cauê Sousa - Desenvolvedor Back-end Java" />
            
          <div
            class="absolute -bottom-3 left-1/2 -translate-x-1/2 bg-white shadow-lg border border-gray-100 rounded-full px-5 py-2 whitespace-nowrap">
            <span class="text-xs font-bold uppercase text-[#2c3e50]">
              Java • Spring Boot
            </span>
          </div>
        </div>
      </div>
    </section>
  </header>
</template>

<script setup>
import { ref } from "vue";

const menuNav = ref(false);

const closeMenu = () => {
  menuNav.value = false;
};

const visualizarCurriculo = () => {
  window.open("/currículo-caue.pdf", "_blank");
};
</script>

<style scoped>
.menu-enter-active,
.menu-leave-active {
  transition: opacity 0.25s ease, transform 0.25s ease;
}

.menu-enter-from,
.menu-leave-to {
  opacity: 0;
  transform: translateX(100%);
}
</style>