<template>
  <header class="container m-auto">
    <nav class="flex justify-center items-center py-3 px-5 font-bold">
      <ul
        class="sm:flex items-center gap-4 hidden uppercase text-sm py-3 px-6 shadow-lg border border-gray-100 rounded-full"
      >
        <li>
          <a
            href="#skills"
            class="hover:text-sm hover:text-[#79BFFA] hover:underline underline-offset-4 decoration-2 decoration-[#79BFFA] transition-all"
            >Skills</a
          >
        </li>
        <li>
          <a
            href="#project"
            class="hover:text-sm hover:text-[#79BFFA] hover:underline underline-offset-4 decoration-2 decoration-[#79BFFA] transition-all"
            >Projetos</a
          >
        </li>
        <li>
          <a
            href="#contact"
            class="hover:text-sm hover:text-[#79BFFA] hover:underline underline-offset-4 decoration-2 decoration-[#79BFFA] transition-all"
            >Contato</a
          >
        </li>
      </ul>
    </nav>

    <div class="flex justify-end sm:hidden">
      <button
        v-on:click="menuNav = !menuNav"
        class="text-[#2c3e50] mx-4 cursor-pointer hover:scale-95 transition-all"
      >
        <svg
          xmlns="http://www.w3.org/2000/svg"
          width="24"
          height="24"
          viewBox="0 0 24 24"
          fill="none"
          stroke="currentColor"
          stroke-width="2"
          stroke-linecap="round"
          stroke-linejoin="round"
          class="lucide lucide-menu-icon lucide-menu"
        >
          <path d="M4 5h16" />
          <path d="M4 12h16" />
          <path d="M4 19h16" />
        </svg>
      </button>
    </div>

    <nav
      v-show="menuNav"
      v-bind:class="
        menuNav === true
          ? 'fixed top-0 z-50 bg-white border-r border-gray-100 w-72 h-full sm:hidden'
          : ''
      "
    >
      <ul class="p-2 text-start uppercase">
        <li class="flex justify-between">
          <h1 class="text-[#2c3e50] font-bold">Menu</h1>
          <button v-on:click="menuNav = false">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              width="24"
              height="24"
              viewBox="0 0 24 24"
              fill="none"
              stroke="currentColor"
              stroke-width="2"
              stroke-linecap="round"
              stroke-linejoin="round"
              class="lucide lucide-x-icon lucide-x"
            >
              <path d="M18 6 6 18" />
              <path d="m6 6 12 12" />
            </svg>
          </button>
        </li>

        <div class="bg-gray-100 p-[1px] rounded-full my-4"></div>

        <li>
          <a
            href="#skills"
            class="hover:text-sm hover:text-[#79BFFA] hover:underline underline-offset-4 decoration-2 decoration-[#79BFFA] transition-all"
            >Skills</a
          >
        </li>
        <li>
          <a
            href="#project"
            class="hover:text-sm hover:text-[#79BFFA] hover:underline underline-offset-4 decoration-2 decoration-[#79BFFA] transition-all"
            >Projetos</a
          >
        </li>
        <li>
          <a
            href="#contact"
            class="hover:text-sm hover:text-[#79BFFA] hover:underline underline-offset-4 decoration-2 decoration-[#79BFFA] transition-all"
            >Contato</a
          >
        </li>
      </ul>
    </nav>

    <section class="font-bold grid lg:grid-cols-2 items-center py-3 px-5">
      <div class="text-start space-y-10">
        <div class="text-start space-y-2">
          <h3 class="mx-2 uppercase text-xs">Olá, me chamo</h3>
          <h1 class="text-3xl sm:text-6xl uppercase">Cauê Sousa</h1>
          <h3 class="mx-2 uppercase text-sm">
            Desenvolvedor full-stack | PHP | Laravel | JavaScript | Java
          </h3>
        </div>

        <!-- <p class="text-sm text-gray-600 ml-1 sm:mr-46">
          Sou desenvolvedor com experiência no desenvolvimento de aplicações web
          modernas e escaláveis, atuando tanto no frontend quanto no backend
        </p> -->

        <div class="flex items-center gap-4">
          <a
            @click="visualizarCurriculo"
            class="text-white text-sm uppercase bg-[#2c3e50] py-2 px-5 rounded cursor-pointer hover:scale-95 transition-all"
          >
            Download CV
          </a>

          <div class="flex space-x-4">
            <button
              onclick="window.open('https://github.com/w-Caue', '_blank')"
              class="flex items-center gap-2 text-white text-sm uppercase py-2 px-5 bg-[#2c3e50] cursor-pointer rounded-full hover:scale-95 transition-all"
            >
              <svg
                xmlns="http://www.w3.org/2000/svg"
                width="24"
                height="24"
                viewBox="0 0 24 24"
                fill="none"
                stroke="currentColor"
                stroke-width="2"
                stroke-linecap="round"
                stroke-linejoin="round"
                class="lucide lucide-github-icon lucide-github"
              >
                <path
                  d="M15 22v-4a4.8 4.8 0 0 0-1-3.5c3 0 6-2 6-5.5.08-1.25-.27-2.48-1-3.5.28-1.15.28-2.35 0-3.5 0 0-1 0-3 1.5-2.64-.5-5.36-.5-8 0C6 2 5 2 5 2c-.3 1.15-.3 2.35 0 3.5A5.403 5.403 0 0 0 4 9c0 3.5 3 5.5 6 5.5-.39.49-.68 1.05-.85 1.65-.17.6-.22 1.23-.15 1.85v4"
                />
                <path d="M9 18c-4.51 2-5-2-7-2" />
              </svg>
              <span class="hidden sm:block">GitHub</span>
            </button>

            <button
              onclick="window.open('https://www.linkedin.com/in/cauesousadev/', '_blank')"
              class="flex items-center gap-2 text-white text-sm uppercase py-2 px-5 bg-[#2c3e50] cursor-pointer rounded-full hover:scale-95 transition-all"
            >
              <svg
                xmlns="http://www.w3.org/2000/svg"
                width="24"
                height="24"
                viewBox="0 0 24 24"
                fill="none"
                stroke="currentColor"
                stroke-width="2"
                stroke-linecap="round"
                stroke-linejoin="round"
                class="lucide lucide-linkedin-icon lucide-linkedin"
              >
                <path
                  d="M16 8a6 6 0 0 1 6 6v7h-4v-7a2 2 0 0 0-2-2 2 2 0 0 0-2 2v7h-4v-7a6 6 0 0 1 6-6z"
                />
                <rect width="4" height="12" x="2" y="9" />
                <circle cx="4" cy="4" r="2" />
              </svg>

              <span class="hidden sm:block">linkedin</span>
            </button>
          </div>
        </div>
      </div>

      <div class="flex justify-center mt-4 sm:mt-0">
        <img
          class="rounded-full"
          src="../assets/img/ft-caue.png"
          alt="modelo"
        />
      </div>
    </section>
  </header>
</template>

<script setup>
import { ref } from "vue";

const menuNav = ref(false);

const visualizarCurriculo = () => {
  window.open("/currículo-caue.pdf", "_blank");
};
</script>

<style></style>
