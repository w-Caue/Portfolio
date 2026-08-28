<template>
  <section id="project" class="container mx-auto px-5 py-24 font-bold">

    <div class="max-w-3xl mb-12">
      <span class="inline-flex items-center gap-2 text-xs uppercase tracking-widest text-[#79BFFA]">
        <span class="w-2 h-2 bg-[#79BFFA] rounded-full"></span>
        Projetos
      </span>

      <h2 class="mt-3 text-3xl sm:text-4xl lg:text-5xl uppercase text-[#2c3e50] leading-tight">
        Projetos que transformam
        <span class="text-[#79BFFA]">
          código em soluções.
        </span>
      </h2>

      <p class="mt-5 text-sm sm:text-base text-gray-500 font-normal leading-relaxed max-w-2xl">
        Alguns dos projetos que desenvolvi durante minha jornada como
        desenvolvedor, aplicando conceitos de arquitetura, APIs REST,
        banco de dados, segurança e desenvolvimento web.
      </p>
    </div>

    <Swiper :modules="modules" :slides-per-view="1" :space-between="24" :breakpoints="{
      768: {
        slidesPerView: 2,
      },
      1024: {
        slidesPerView: 3,
      },
    }" :navigation="{
      nextEl: '.project-next',
      prevEl: '.project-prev',
    }" class="projects-swiper">

      <div class="flex items-center justify-center gap-3 mt-8">

        <!-- Voltar -->
        <button class="project-prev group flex items-center justify-center
           w-12 h-12 rounded-full
           border border-gray-200 bg-white
           text-[#2c3e50]
           shadow-sm
           hover:bg-[#79BFFA]
           hover:border-[#79BFFA]
           hover:-translate-x-1
           transition-all duration-300
           cursor-pointer" aria-label="Projeto anterior">
          <i class="fa-solid fa-arrow-left
             text-sm
             group-hover:text-[#2c3e50]
             transition-all"></i>
        </button>

        <!-- Próximo -->
        <button class="project-next group flex items-center justify-center
           w-12 h-12 rounded-full
           bg-[#2c3e50]
           text-white
           shadow-sm
           hover:bg-[#79BFFA]
           hover:text-[#2c3e50]
           hover:translate-x-1
           transition-all duration-300
           cursor-pointer" aria-label="Próximo projeto">
          <i class="fa-solid fa-arrow-right
             text-sm
             transition-all"></i>
        </button>

      </div>

      <SwiperSlide>
        <article
          class="group h-full bg-white border border-gray-100 rounded-2xl overflow-hidden shadow-sm hover:shadow-xl transition-all duration-300">
        
          <div class="relative h-56 bg-gray-100 overflow-hidden">
            <img src="../assets/projects/project-1.png"
              alt="Sistema de gerenciamento desenvolvido com Java e Spring Boot"
              class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-500" />

            <div class="absolute top-4 left-4 bg-[#2c3e50] text-white text-[10px] uppercase px-3 py-1.5 rounded-full">
              Java / Back-end
            </div>
          </div>

          <div class="p-6">

            <h3 class="text-xl uppercase text-[#2c3e50]">
              Sistema de Gerenciamento
            </h3>

            <p class="mt-3 text-sm text-gray-500 font-normal leading-relaxed">
              Aplicação desenvolvida para gerenciamento de usuários,
              produtos e pedidos, utilizando uma arquitetura organizada
              e uma API REST.
            </p>

            <div class="mt-5 space-y-2">
              <div class="flex items-center gap-2 text-xs text-gray-500 font-normal">
                <i class="fa-solid fa-check text-[#79BFFA]"></i>
                Autenticação e autorização
              </div>

              <div class="flex items-center gap-2 text-xs text-gray-500 font-normal">
                <i class="fa-solid fa-check text-[#79BFFA]"></i>
                CRUD completo
              </div>

              <div class="flex items-center gap-2 text-xs text-gray-500 font-normal">
                <i class="fa-solid fa-check text-[#79BFFA]"></i>
                Integração com MySQL
              </div>
            </div>

            <div class="flex flex-wrap gap-2 mt-6">

              <span
                class="flex items-center gap-1.5 text-[10px] uppercase bg-gray-50 border border-gray-100 px-3 py-1.5 rounded-full">
                <i class="devicon-java-plain colored"></i>
                Java
              </span>

              <span
                class="flex items-center gap-1.5 text-[10px] uppercase bg-gray-50 border border-gray-100 px-3 py-1.5 rounded-full">
                <i class="devicon-spring-original colored"></i>
                Spring Boot
              </span>

              <span
                class="flex items-center gap-1.5 text-[10px] uppercase bg-gray-50 border border-gray-100 px-3 py-1.5 rounded-full">
                <i class="devicon-mysql-original colored"></i>
                MySQL
              </span>

            </div>

            <div class="flex items-center gap-3 mt-7">

              <a href="#" target="_blank"
                class="flex items-center gap-2 text-xs uppercase text-white bg-[#2c3e50] px-5 py-2.5 rounded-full hover:bg-[#79BFFA] hover:text-[#2c3e50] transition-all">
                <i class="fa-brands fa-github"></i>
                GitHub
              </a>

              <a href="#" target="_blank"
                class="flex items-center gap-2 text-xs uppercase text-[#2c3e50] border border-gray-200 px-5 py-2.5 rounded-full hover:border-[#79BFFA] hover:bg-[#79BFFA] transition-all">
                <i class="fa-solid fa-arrow-up-right-from-square"></i>
                Demo
              </a>

            </div>
          </div>
        </article>
      </SwiperSlide>

      <SwiperSlide>
        <article
          class="group h-full bg-white border border-gray-100 rounded-2xl overflow-hidden shadow-sm hover:shadow-xl transition-all duration-300">

          <div class="relative h-56 bg-gray-100 overflow-hidden">
            <img src="../assets/projects/project-2.png" alt="API REST desenvolvida com Java e Spring Boot"
              class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-500" />

            <div class="absolute top-4 left-4 bg-[#2c3e50] text-white text-[10px] uppercase px-3 py-1.5 rounded-full">
              Java / API
            </div>
          </div>

          <div class="p-6">

            <h3 class="text-xl uppercase text-[#2c3e50]">
              API REST
            </h3>

            <p class="mt-3 text-sm text-gray-500 font-normal leading-relaxed">
              API REST desenvolvida com Spring Boot para gerenciamento
              de recursos, utilizando boas práticas de desenvolvimento
              e persistência de dados.
            </p>

            <div class="mt-5 space-y-2">

              <div class="flex items-center gap-2 text-xs text-gray-500 font-normal">
                <i class="fa-solid fa-check text-[#79BFFA]"></i>
                Endpoints REST
              </div>

              <div class="flex items-center gap-2 text-xs text-gray-500 font-normal">
                <i class="fa-solid fa-check text-[#79BFFA]"></i>
                Validação de dados
              </div>

              <div class="flex items-center gap-2 text-xs text-gray-500 font-normal">
                <i class="fa-solid fa-check text-[#79BFFA]"></i>
                Banco de dados relacional
              </div>

            </div>

            <div class="flex flex-wrap gap-2 mt-6">

              <span
                class="flex items-center gap-1.5 text-[10px] uppercase bg-gray-50 border border-gray-100 px-3 py-1.5 rounded-full">
                <i class="devicon-java-plain colored"></i>
                Java
              </span>

              <span
                class="flex items-center gap-1.5 text-[10px] uppercase bg-gray-50 border border-gray-100 px-3 py-1.5 rounded-full">
                <i class="devicon-spring-original colored"></i>
                Spring Boot
              </span>

              <span
                class="flex items-center gap-1.5 text-[10px] uppercase bg-gray-50 border border-gray-100 px-3 py-1.5 rounded-full">
                REST
              </span>

            </div>

            <div class="flex items-center gap-3 mt-7">

              <a href="#" target="_blank"
                class="flex items-center gap-2 text-xs uppercase text-white bg-[#2c3e50] px-5 py-2.5 rounded-full hover:bg-[#79BFFA] hover:text-[#2c3e50] transition-all">
                <i class="fa-brands fa-github"></i>
                GitHub
              </a>

              <a href="#" target="_blank"
                class="flex items-center gap-2 text-xs uppercase text-[#2c3e50] border border-gray-200 px-5 py-2.5 rounded-full hover:border-[#79BFFA] hover:bg-[#79BFFA] transition-all">
                <i class="fa-solid fa-arrow-up-right-from-square"></i>
                Demo
              </a>

            </div>

          </div>
        </article>
      </SwiperSlide>

      <SwiperSlide>
        <article
          class="group h-full bg-white border border-gray-100 rounded-2xl overflow-hidden shadow-sm hover:shadow-xl transition-all duration-300">

          <div class="relative h-56 bg-gray-100 overflow-hidden">
            <img src="../assets/projects/project-3.png" alt="Aplicação web desenvolvida com Laravel e Vue.js"
              class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-500" />

            <div class="absolute top-4 left-4 bg-[#2c3e50] text-white text-[10px] uppercase px-3 py-1.5 rounded-full">
              Full Stack
            </div>
          </div>

          <div class="p-6">

            <h3 class="text-xl uppercase text-[#2c3e50]">
              Aplicação Web
            </h3>

            <p class="mt-3 text-sm text-gray-500 font-normal leading-relaxed">
              Aplicação web desenvolvida utilizando Laravel no Back-end
              e Vue.js no Front-end, com integração através de APIs.
            </p>

            <div class="mt-5 space-y-2">

              <div class="flex items-center gap-2 text-xs text-gray-500 font-normal">
                <i class="fa-solid fa-check text-[#79BFFA]"></i>
                Interface responsiva
              </div>

              <div class="flex items-center gap-2 text-xs text-gray-500 font-normal">
                <i class="fa-solid fa-check text-[#79BFFA]"></i>
                API REST
              </div>

              <div class="flex items-center gap-2 text-xs text-gray-500 font-normal">
                <i class="fa-solid fa-check text-[#79BFFA]"></i>
                Banco de dados MySQL
              </div>

            </div>

            <div class="flex flex-wrap gap-2 mt-6">

              <span
                class="flex items-center gap-1.5 text-[10px] uppercase bg-gray-50 border border-gray-100 px-3 py-1.5 rounded-full">
                <i class="devicon-laravel-original colored"></i>
                Laravel
              </span>

              <span
                class="flex items-center gap-1.5 text-[10px] uppercase bg-gray-50 border border-gray-100 px-3 py-1.5 rounded-full">
                <i class="devicon-vuejs-plain colored"></i>
                Vue.js
              </span>

              <span
                class="flex items-center gap-1.5 text-[10px] uppercase bg-gray-50 border border-gray-100 px-3 py-1.5 rounded-full">
                <i class="devicon-mysql-original colored"></i>
                MySQL
              </span>

            </div>

            <div class="flex items-center gap-3 mt-7">

              <a href="#" target="_blank"
                class="flex items-center gap-2 text-xs uppercase text-white bg-[#2c3e50] px-5 py-2.5 rounded-full hover:bg-[#79BFFA] hover:text-[#2c3e50] transition-all">
                <i class="fa-brands fa-github"></i>
                GitHub
              </a>

              <a href="#" target="_blank"
                class="flex items-center gap-2 text-xs uppercase text-[#2c3e50] border border-gray-200 px-5 py-2.5 rounded-full hover:border-[#79BFFA] hover:bg-[#79BFFA] transition-all">
                <i class="fa-solid fa-arrow-up-right-from-square"></i>
                Demo
              </a>

            </div>

          </div>
        </article>
      </SwiperSlide>

    </Swiper>

    <div class="mt-10 flex items-center justify-center gap-2 text-xs uppercase text-gray-400">
      <i class="fa-solid fa-arrow-left"></i>

      <span>
        Arraste para explorar
      </span>

      <i class="fa-solid fa-arrow-right"></i>
    </div>

  </section>
</template>

<script setup>
import { Swiper, SwiperSlide } from "swiper/vue";
import { Navigation, Pagination } from "swiper/modules";

import "swiper/css";
import "swiper/css/navigation";
import "swiper/css/pagination";

const modules = [Navigation, Pagination];
</script>