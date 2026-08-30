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

            <img src="../assets/projects/project-product.png" alt="Preview do site desenvolvido para empresa"
              class="w-full h-full object-cover object-top group-hover:scale-105 transition-transform duration-500" />

            <div class="absolute inset-0 bg-[#2c3e50]/0 group-hover:bg-[#2c3e50]/20 transition-all duration-300"></div>

            <div class="absolute top-4 left-4">
              <span
                class="flex items-center gap-2 bg-[#2c3e50]/90 backdrop-blur-sm text-white text-[10px] uppercase px-3 py-1.5 rounded-full">
                <span class="w-1.5 h-1.5 bg-[#79BFFA] rounded-full"></span>
                Sistema Online
              </span>
            </div>

            <div class="absolute top-4 right-4">
              <span
                class="flex items-center gap-2 bg-white/90 backdrop-blur-sm text-[#2c3e50] text-[9px] uppercase px-3 py-1.5 rounded-full">
                <i class="fa-solid fa-globe"></i>
                Online
              </span>
            </div>

          </div>

          <div class="p-6">

            <div class="flex items-start justify-between gap-4">

              <div>
                <span class="text-[9px] uppercase tracking-widest text-[#79BFFA]">
                  Front-end + Back-end
                </span>

                <h3 class="text-xl uppercase text-[#2c3e50]">
                  Product Manager - sistema
                </h3>
              </div>

              <div class="flex items-center justify-center w-9 h-9 rounded-full bg-gray-50">
                <i class="fa-solid fa-globe text-sm text-[#2c3e50]"></i>
              </div>

            </div>

            <p class="mt-4 text-sm text-gray-500 font-normal leading-relaxed">
              Sistema web para gerenciamento de produtos, desenvolvido com Vue.js no frontend e Java + Spring Boot no
              backend. O projeto foi desenvolvido com foco em demonstrar na prática a construção de uma aplicação full
              stack.
            </p>

            <div class="mt-5 space-y-2">

              <div class="flex items-center gap-2 text-xs text-gray-500 font-normal">
                <i class="fa-solid fa-check text-[#79BFFA]"></i>
                Design responsivo
              </div>

              <div class="flex items-center gap-2 text-xs text-gray-500 font-normal">
                <i class="fa-solid fa-check text-[#79BFFA]"></i>
                Autenticação JWT
              </div>

              <div class="flex items-center gap-2 text-xs text-gray-500 font-normal">
                <i class="fa-solid fa-check text-[#79BFFA]"></i>
                Operações CRUD
              </div>

              <div class="flex items-center gap-2 text-xs text-gray-500 font-normal">
                <i class="fa-solid fa-check text-[#79BFFA]"></i>
                consumo de API REST
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
                <i class="devicon-vuejs-plain colored"></i>
                Vue.js
              </span>

              <span
                class="flex items-center gap-1.5 text-[10px] uppercase bg-gray-50 border border-gray-100 px-3 py-1.5 rounded-full">
                <i class="devicon-tailwindcss-plain colored"></i>
                Tailwind CSS
              </span>

              <span
                class="flex items-center gap-1.5 text-[10px] uppercase bg-gray-50 border border-gray-100 px-3 py-1.5 rounded-full">
                <i class="devicon-mysql-plain colored"></i>
                MySQL
              </span>

            </div>

            <div class="flex items-center gap-3 mt-7">
              <a href="https://product-front.netlify.app/" target="_blank" rel="noopener noreferrer"
                class="flex items-center gap-2 text-xs uppercase text-white bg-[#2c3e50] px-5 py-2.5 rounded-full hover:bg-[#79BFFA] hover:text-[#2c3e50] transition-all">
                <i class="fa-solid fa-arrow-up-right-from-square"></i>
                Demo
              </a>

              <a href="https://github.com/w-Caue/front-product-erp" target="_blank" rel="noopener noreferrer"
                class="flex items-center gap-2 text-xs uppercase text-[#2c3e50] border border-gray-200 px-5 py-2.5 rounded-full hover:border-[#79BFFA] hover:bg-[#79BFFA] transition-all">
                <i class="fa-brands fa-github"></i>
                github
              </a>

            </div>

          </div>
        </article>
      </SwiperSlide>

      <SwiperSlide>
        <article
          class="group h-full bg-white border border-gray-100 rounded-2xl overflow-hidden shadow-sm hover:shadow-xl transition-all duration-300">

          <div class="relative h-56 bg-[#2c3e50] overflow-hidden">

            <div class="absolute -right-16 -top-16 w-40 h-40 rounded-full border border-[#79BFFA]/10"></div>

            <div class="absolute -left-20 -bottom-20 w-48 h-48 rounded-full border border-[#79BFFA]/10"></div>
            <div class="relative h-full flex flex-col justify-center px-6">
              <div class="flex items-center gap-3">

                <i class="devicon-java-plain text-4xl text-[#79BFFA]"></i>

                <i class="devicon-spring-original text-4xl text-[#79BFFA]"></i>

                <div class="h-8 w-px bg-white/10"></div>

                <span class="text-[10px] uppercase tracking-[0.2em] text-gray-300">
                  Back-end
                </span>

              </div>

              <!-- Endpoints -->
              <div class="mt-5 space-y-1.5 font-mono text-[10px]">

                <div class="flex items-center gap-2">
                  <span class="text-[#79BFFA] w-10">
                    GET
                  </span>

                  <span class="text-gray-400">
                    /agendamentos
                  </span>

                  <span class="text-green-400 ml-auto">
                    200
                  </span>
                </div>

                <div class="flex items-center gap-2">
                  <span class="text-[#79BFFA] w-10">
                    POST
                  </span>

                  <span class="text-gray-400">
                    /agendamentos
                  </span>

                  <span class="text-green-400 ml-auto">
                    201
                  </span>
                </div>

                <div class="flex items-center gap-2">
                  <span class="text-[#79BFFA] w-10">
                    PUT
                  </span>

                  <span class="text-gray-400">
                    /agendamentos/{cliente}
                  </span>

                  <span class="text-green-400 ml-auto">
                    200
                  </span>
                </div>

                <div class="flex items-center gap-2">
                  <span class="text-[#79BFFA] w-10">
                    DELETE
                  </span>

                  <span class="text-gray-400">
                    /agendamentos/{cliente}
                  </span>

                  <span class="text-green-400 ml-auto">
                    204
                  </span>
                </div>

              </div>

              <div class="absolute top-4 right-4">
                <span
                  class="flex items-center gap-2 bg-white/10 backdrop-blur-sm border border-white/10 text-white text-[9px] uppercase px-3 py-1.5 rounded-full">
                  <span class="w-1.5 h-1.5 rounded-full bg-[#79BFFA]"></span>

                  REST API
                </span>
              </div>

            </div>
          </div>

          <div class="p-6">

            <div class="flex items-start justify-between gap-4">

              <div>
                <span class="text-[9px] uppercase tracking-widest text-[#79BFFA]">
                  Backend
                </span>

                <h3 class="mt-1 text-xl uppercase text-[#2c3e50]">
                  Agendamentos - API REST
                </h3>
              </div>

              <div class="flex items-center justify-center w-9 h-9 rounded-full bg-gray-50">
                <i class="fa-solid fa-server text-sm text-[#2c3e50]"></i>
              </div>

            </div>

            <p class="mt-4 text-sm text-gray-500 font-normal leading-relaxed">
              API REST desenvolvida com Java e Spring Boot para
              um controle de agendamentos, aplicando arquitetura em
              camadas, validação de dados e persistência com banco
              de dados relacional.
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
                Arquitetura em camadas
              </div>

              <div class="flex items-center gap-2 text-xs text-gray-500 font-normal">
                <i class="fa-solid fa-check text-[#79BFFA]"></i>
                Persistência de dados
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
                <i class="devicon-hibernate-plain colored"></i>
                JPA
              </span>

              <span
                class="flex items-center gap-1.5 text-[10px] uppercase bg-gray-50 border border-gray-100 px-3 py-1.5 rounded-full">
                <i class="devicon-mysql-plain colored"></i>
                MySQL
              </span>

            </div>

            <div class="flex items-center gap-3 mt-7">

              <a href="https://github.com/w-Caue/controle-agendamentos" target="_blank" rel="noopener noreferrer"
                class="flex items-center gap-2 text-xs uppercase text-white bg-[#2c3e50] px-5 py-2.5 rounded-full hover:bg-[#79BFFA] hover:text-[#2c3e50] transition-all">
                <i class="fa-brands fa-github"></i>
                GitHub
              </a>

              <!-- <a href="#" target="_blank" rel="noopener noreferrer"
                class="flex items-center gap-2 text-xs uppercase text-[#2c3e50] border border-gray-200 px-5 py-2.5 rounded-full hover:border-[#79BFFA] hover:bg-[#79BFFA] transition-all">
                <i class="fa-solid fa-book-open"></i>
                Documentação
              </a> -->

            </div>

          </div>
        </article>
      </SwiperSlide>

      <SwiperSlide>
        <article
          class="group h-full bg-white border border-gray-100 rounded-2xl overflow-hidden shadow-sm hover:shadow-xl transition-all duration-300">

          <div class="relative h-56 bg-gray-100 overflow-hidden">

            <img src="../assets/projects/project-codestudio.png" alt="Preview do site desenvolvido para empresa"
              class="w-full h-full object-cover object-top group-hover:scale-105 transition-transform duration-500" />

            <div class="absolute inset-0 bg-[#2c3e50]/0 group-hover:bg-[#2c3e50]/20 transition-all duration-300"></div>

            <div class="absolute top-4 left-4">
              <span
                class="flex items-center gap-2 bg-[#2c3e50]/90 backdrop-blur-sm text-white text-[10px] uppercase px-3 py-1.5 rounded-full">
                <span class="w-1.5 h-1.5 bg-[#79BFFA] rounded-full"></span>
                Site Online
              </span>
            </div>

            <div class="absolute top-4 right-4">
              <span
                class="flex items-center gap-2 bg-white/90 backdrop-blur-sm text-[#2c3e50] text-[9px] uppercase px-3 py-1.5 rounded-full">
                <i class="fa-solid fa-globe"></i>
                Online
              </span>
            </div>

          </div>

          <div class="p-6">

            <div class="flex items-start justify-between gap-4">

              <div>
                <span class="text-[9px] uppercase tracking-widest text-[#79BFFA]">
                  Front-end
                </span>

                <h3 class="text-xl uppercase text-[#2c3e50]">
                  Code Studio - site
                </h3>
              </div>

              <div class="flex items-center justify-center w-9 h-9 rounded-full bg-gray-50">
                <i class="fa-solid fa-globe text-sm text-[#2c3e50]"></i>
              </div>

            </div>

            <p class="mt-4 text-sm text-gray-500 font-normal leading-relaxed">
              Site institucional desenvolvido com foco em criação de sites, landing pages e sistemas personalizados.
            </p>

            <div class="mt-5 space-y-2">

              <div class="flex items-center gap-2 text-xs text-gray-500 font-normal">
                <i class="fa-solid fa-check text-[#79BFFA]"></i>
                Design responsivo
              </div>

              <div class="flex items-center gap-2 text-xs text-gray-500 font-normal">
                <i class="fa-solid fa-check text-[#79BFFA]"></i>
                Interface moderna
              </div>

              <div class="flex items-center gap-2 text-xs text-gray-500 font-normal">
                <i class="fa-solid fa-check text-[#79BFFA]"></i>
                Otimizado para dispositivos móveis
              </div>

            </div>

            <div class="flex flex-wrap gap-2 mt-6">

              <span
                class="flex items-center gap-1.5 text-[10px] uppercase bg-gray-50 border border-gray-100 px-3 py-1.5 rounded-full">
                <i class="devicon-angularjs-plain colored"></i>
                AngularJs
              </span>

              <span
                class="flex items-center gap-1.5 text-[10px] uppercase bg-gray-50 border border-gray-100 px-3 py-1.5 rounded-full">
                <i class="devicon-tailwindcss-plain colored"></i>
                Tailwind CSS
              </span>

              <span
                class="flex items-center gap-1.5 text-[10px] uppercase bg-gray-50 border border-gray-100 px-3 py-1.5 rounded-full">
                <i class="devicon-javascript-plain colored"></i>
                JavaScript
              </span>

            </div>

            <div class="flex items-center gap-3 mt-7">
              <a href="https://codestudiolabs.netlify.app/" target="_blank" rel="noopener noreferrer"
                class="flex items-center gap-2 text-xs uppercase text-white bg-[#2c3e50] px-5 py-2.5 rounded-full hover:bg-[#79BFFA] hover:text-[#2c3e50] transition-all">
                <i class="fa-solid fa-arrow-up-right-from-square"></i>
                Ver site
              </a>

              <a href="https://github.com/w-Caue/code-studio-labs" target="_blank" rel="noopener noreferrer"
                class="flex items-center gap-2 text-xs uppercase text-[#2c3e50] border border-gray-200 px-5 py-2.5 rounded-full hover:border-[#79BFFA] hover:bg-[#79BFFA] transition-all">
                <i class="fa-brands fa-github"></i>
                github
              </a>

            </div>

          </div>
        </article>
      </SwiperSlide>

      <SwiperSlide>
        <article
          class="group h-full bg-white border border-gray-100 rounded-2xl overflow-hidden shadow-sm hover:shadow-xl transition-all duration-300">

          <div class="relative h-56 bg-gray-100 overflow-hidden">

            <img src="../assets/projects/project-hashem.png" alt="Preview do site desenvolvido para empresa"
              class="w-full h-full object-cover object-top group-hover:scale-105 transition-transform duration-500" />

            <div class="absolute inset-0 bg-[#2c3e50]/0 group-hover:bg-[#2c3e50]/20 transition-all duration-300"></div>

            <div class="absolute top-4 left-4">
              <span
                class="flex items-center gap-2 bg-[#2c3e50]/90 backdrop-blur-sm text-white text-[10px] uppercase px-3 py-1.5 rounded-full">
                <span class="w-1.5 h-1.5 bg-[#79BFFA] rounded-full"></span>
                Site Online
              </span>
            </div>

            <div class="absolute top-4 right-4">
              <span
                class="flex items-center gap-2 bg-white/90 backdrop-blur-sm text-[#2c3e50] text-[9px] uppercase px-3 py-1.5 rounded-full">
                <i class="fa-solid fa-globe"></i>
                Online
              </span>
            </div>

          </div>

          <div class="p-6">

            <div class="flex items-start justify-between gap-4">

              <div>
                <span class="text-[9px] uppercase tracking-widest text-[#79BFFA]">
                  Front-end
                </span>

                <h3 class="text-xl uppercase text-[#2c3e50]">
                  Hashem - site
                </h3>
              </div>

              <div class="flex items-center justify-center w-9 h-9 rounded-full bg-gray-50">
                <i class="fa-solid fa-globe text-sm text-[#2c3e50]"></i>
              </div>

            </div>

            <p class="mt-4 text-sm text-gray-500 font-normal leading-relaxed">
              Site desenvolvido para uma academia de jiu-jistu e muay thai com foco em formar atletas e cidadãos através
              da disciplina, respeito e perseverança.
            </p>

            <div class="mt-5 space-y-2">

              <div class="flex items-center gap-2 text-xs text-gray-500 font-normal">
                <i class="fa-solid fa-check text-[#79BFFA]"></i>
                Design responsivo
              </div>

              <div class="flex items-center gap-2 text-xs text-gray-500 font-normal">
                <i class="fa-solid fa-check text-[#79BFFA]"></i>
                Tecnologias de alta performace
              </div>

              <div class="flex items-center gap-2 text-xs text-gray-500 font-normal">
                <i class="fa-solid fa-check text-[#79BFFA]"></i>
                Otimizado para dispositivos móveis
              </div>

            </div>

            <div class="flex flex-wrap gap-2 mt-6">

              <span
                class="flex items-center gap-1.5 text-[10px] uppercase bg-gray-50 border border-gray-100 px-3 py-1.5 rounded-full">
                <i class="devicon-vuejs-plain colored"></i>
                Vue.js
              </span>

              <span
                class="flex items-center gap-1.5 text-[10px] uppercase bg-gray-50 border border-gray-100 px-3 py-1.5 rounded-full">
                <i class="devicon-tailwindcss-plain colored"></i>
                Tailwind CSS
              </span>

            </div>

            <div class="flex items-center gap-3 mt-7">
              <a href="https://hashemyhwh.netlify.app" target="_blank" rel="noopener noreferrer"
                class="flex items-center gap-2 text-xs uppercase text-white bg-[#2c3e50] px-5 py-2.5 rounded-full hover:bg-[#79BFFA] hover:text-[#2c3e50] transition-all">
                <i class="fa-solid fa-arrow-up-right-from-square"></i>
                Ver site
              </a>

              <a href="https://github.com/w-Caue/hashem-site" target="_blank" rel="noopener noreferrer"
                class="flex items-center gap-2 text-xs uppercase text-[#2c3e50] border border-gray-200 px-5 py-2.5 rounded-full hover:border-[#79BFFA] hover:bg-[#79BFFA] transition-all">
                <i class="fa-brands fa-github"></i>
                github
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