<template>
  <section id="project" class="font-bold py-3 px-5 mx-2 my-16">
    <div class="">
      <h1 class="text-3xl">
        Meus <span class="text-[#79BFFA]">Projetos</span>
      </h1>
    </div>

    <!-- Carrossel de Produtos -->
    <Swiper
      :modules="[Navigation, Pagination]"
      :slides-per-view="4"
      :space-between="1"
      :loop="true"
      :navigation="{ nextEl: '.button-next', prevEl: '.button-prev' }"
      :breakpoints="{
        320: { slidesPerView: 1 },
        640: { slidesPerView: 2 },
        1024: { slidesPerView: 4 },
        1440: { slidesPerView: 5 },
      }"
      class="relative"
    >
      <SwiperSlide v-for="(project, index) in projects" :key="index">
        <div class="bg-white w-72 rounded-xl p-4 mx-auto cursor-pointer">
          <!-- Carrossel de imagens do produto -->
          <Swiper
            :modules="[Navigation]"
            :slides-per-view="1"
            :loop="true"
            :navigation="{ nextEl: '.custom-next', prevEl: '.custom-prev' }"
            class="rounded-lg mb-4 relative"
          >
            <SwiperSlide v-for="(image, i) in project.images" :key="i">
              <img
                :src="image"
                :alt="project.title"
                class="w-full h-72 object-cover rounded-lg"
              />
            </SwiperSlide>
            <button
              class="custom-prev absolute z-10 top-1/2 left-1 transform -translate-y-1/2 text-white p-1 rounded-full hover:bg-[#79BFFA] cursor-pointer"
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
                class="lucide lucide-chevron-left-icon lucide-chevron-left"
              >
                <path d="m15 18-6-6 6-6" />
              </svg>
            </button>
            <button
              class="custom-next absolute z-10 top-1/2 right-1 transform -translate-y-1/2 text-white p-1 rounded-full hover:bg-[#79BFFA] cursor-pointer"
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
                class="lucide lucide-chevron-right-icon lucide-chevron-right"
              >
                <path d="m9 18 6-6-6-6" />
              </svg>
            </button>
          </Swiper>

          <!-- Informações do produto -->
          <div @click="openLink(project.link)" class="text-start font-bold">
            <h2 class="text-sm text-gray-500">{{ project.title }}</h2>
            <p class="">
              {{ project.description }}
            </p>

            <h3 class="text-sm text-[#79BFFA]">
              {{ project.languages }}
            </h3>
          </div>
        </div>
      </SwiperSlide>

      <button
        class="button-prev absolute z-10 top-1/2 left-1 transform -translate-y-1/2 text-[#79BFFA] bg-gray-100 shadow-md p-1 rounded-full hover:bg-gray-200 cursor-pointer"
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
          class="lucide lucide-chevron-left-icon lucide-chevron-left"
        >
          <path d="m15 18-6-6 6-6" />
        </svg>
      </button>
      <button
        class="button-next absolute z-10 top-1/2 right-1 transform -translate-y-1/2 text-[#79BFFA] bg-gray-100 shadow-md p-1 rounded-full hover:bg-gray-200 cursor-pointer"
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
          class="lucide lucide-chevron-right-icon lucide-chevron-right"
        >
          <path d="m9 18 6-6-6-6" />
        </svg>
      </button>
    </Swiper>
  </section>
</template>

<script></script>

<script setup>
import { Swiper, SwiperSlide } from "swiper/vue";
import { Navigation, Pagination } from "swiper/modules";

// Import Swiper CSS
import "swiper/css";
import "swiper/css/navigation";
import "swiper/css/pagination";

const projects = [
  {
    title: "Site",
    description: "IKIN Performace",
    languages: "VueJs / Tailwind",
    link: "https://ikin.netlify.app",
    images: [new URL("@/assets/projects/logo-ikin.jpeg", import.meta.url).href],
  },
  {
    title: "Sistema",
    description: "Kanban",
    languages: "Laravel / Livewire / Tailwind",
    link: "https://github.com/w-Caue",
    images: [new URL("@/assets/projects/padrao.png", import.meta.url).href],
  },
  {
    title: "Sistema",
    description: "Ecommerce",
    languages: "Laravel / Livewire / Tailwind",
    link: "https://github.com/w-Caue/ecommerce-laravel",
    images: [new URL("@/assets/projects/padrao.png", import.meta.url).href],
  },
  {
    title: "Sistema",
    description: "Cadastro",
    languages: "Java / Spring Boot",
    link: "https://github.com/w-Caue/cadastro-usuario",
    images: [new URL("@/assets/projects/padrao.png", import.meta.url).href],
  },
  {
    title: "Sistema",
    description: "Comercial",
    languages: "Java",
    link: "https://github.com/w-Caue/SistemaComercial",
    images: [new URL("@/assets/projects/padrao.png", import.meta.url).href],
  },
  {
    title: "Landing Page",
    description: "Landing Page Hamburguer",
    languages: "Html / Css / JavaScript",
    link: "https://w-caue.github.io/LandingPage-Hamburguer/",
    images: [new URL("@/assets/projects/padrao.png", import.meta.url).href],
  },
];

function openLink(url) {
  const fullUrl = url.startsWith("http") ? url : `https://${url}`;
  window.open(fullUrl, "_blank");
}
</script>
