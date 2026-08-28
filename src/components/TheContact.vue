<template>
  <section id="contact" class="container mx-auto px-5 py-24 font-bold">
    <div class="relative overflow-hidden rounded-3xl bg-[#2c3e50] px-6 py-12 sm:px-10 lg:px-16 lg:py-16">
      <div class="absolute -right-20 -top-20 h-64 w-64 rounded-full border border-[#79BFFA]/10"></div>

      <div class="absolute -right-8 -top-8 h-40 w-40 rounded-full border border-[#79BFFA]/10"></div>

      <div class="absolute -bottom-24 -left-24 h-64 w-64 rounded-full bg-[#79BFFA]/5"></div>

      <div class="relative grid lg:grid-cols-[1fr_auto] gap-10 items-center">

        <div class="max-w-3xl">

          <span class="inline-flex items-center gap-2 text-xs uppercase tracking-widest text-[#79BFFA]">
            <span class="h-2 w-2 rounded-full bg-[#79BFFA]"></span>

            Vamos conversar
          </span>

          <h2 class="mt-4 text-3xl sm:text-4xl lg:text-5xl uppercase leading-tight text-white">
            Tem um projeto em mente?
            <span class="text-[#79BFFA]">
              Vamos construir juntos.
            </span>
          </h2>

          <p class="mt-5 max-w-2xl text-sm sm:text-base leading-relaxed text-gray-300 font-normal">
            Estou aberto a novas oportunidades, projetos e desafios.
            Se você está procurando um desenvolvedor para transformar
            uma ideia em uma solução real, entre em contato comigo.
          </p>

          <div class="mt-6 inline-flex items-center gap-3 rounded-full border border-white/10 bg-white/5 px-4 py-2">
            <span class="relative flex h-2.5 w-2.5">
              <span class="absolute inline-flex h-full w-full animate-ping rounded-full bg-[#79BFFA] opacity-75"></span>

              <span class="relative inline-flex h-2.5 w-2.5 rounded-full bg-[#79BFFA]"></span>
            </span>

            <span class="text-[10px] uppercase tracking-widest text-gray-300 font-normal">
              Aberto a novas oportunidades
            </span>
          </div>
        </div>

        <div class="flex flex-col gap-3 w-full lg:w-auto">

          <!-- WhatsApp -->
          <a href="https://wa.me/5585981655691" target="_blank" rel="noopener noreferrer"
            class="group flex items-center justify-between gap-6 rounded-full bg-[#79BFFA] px-6 py-3.5 text-sm uppercase text-[#2c3e50] transition-all duration-300 hover:bg-white hover:translate-x-1">
            <span class="flex items-center gap-3">
              <i class="fa-brands fa-whatsapp text-lg"></i>
              WhatsApp
            </span>

            <i
              class="fa-solid fa-arrow-up-right-from-square text-xs transition-transform group-hover:translate-x-1 group-hover:-translate-y-1"></i>
          </a>

          <!-- LinkedIn -->
          <a href="https://www.linkedin.com/in/cauesousadev/" target="_blank" rel="noopener noreferrer"
            class="group flex items-center justify-between gap-6 rounded-full border border-white/15 bg-white/5 px-6 py-3.5 text-sm uppercase text-white transition-all duration-300 hover:bg-white hover:text-[#2c3e50] hover:translate-x-1">
            <span class="flex items-center gap-3">
              <i class="fa-brands fa-linkedin text-lg"></i>
              LinkedIn
            </span>

            <i
              class="fa-solid fa-arrow-up-right-from-square text-xs transition-transform group-hover:translate-x-1 group-hover:-translate-y-1"></i>
          </a>

          <!-- GitHub -->
          <a href="https://github.com/w-Caue" target="_blank" rel="noopener noreferrer"
            class="group flex items-center justify-between gap-6 rounded-full border border-white/15 bg-white/5 px-6 py-3.5 text-sm uppercase text-white transition-all duration-300 hover:bg-white hover:text-[#2c3e50] hover:translate-x-1">
            <span class="flex items-center gap-3">
              <i class="fa-brands fa-github text-lg"></i>
              GitHub
            </span>

            <i
              class="fa-solid fa-arrow-up-right-from-square text-xs transition-transform group-hover:translate-x-1 group-hover:-translate-y-1"></i>
          </a>

        </div>
      </div>
    </div>

    <div class="grid sm:grid-cols-2 lg:grid-cols-3 gap-4 mt-5">

      <!-- EMAIL -->
      <a href="mailto:seuemail@email.com"
        class="group flex items-center gap-4 rounded-2xl border border-gray-100 bg-gray-50 p-5 transition-all duration-300 hover:bg-white hover:border-[#79BFFA]/50 hover:shadow-md">
        <div class="flex h-11 w-11 shrink-0 items-center justify-center rounded-xl bg-[#79BFFA]/15 text-[#2c3e50]">
          <i class="fa-solid fa-envelope text-lg"></i>
        </div>

        <div class="min-w-0">
          <span class="block text-[10px] uppercase tracking-widest text-gray-400">
            E-mail
          </span>

          <span class="mt-1 block truncate text-sm text-[#2c3e50] group-hover:text-[#79BFFA] transition-colors">
            developercaue@email.com
          </span>
        </div>
      </a>

      <!-- LINKEDIN -->
      <a href="https://www.linkedin.com/in/cauesousadev/" target="_blank" rel="noopener noreferrer"
        class="group flex items-center gap-4 rounded-2xl border border-gray-100 bg-gray-50 p-5 transition-all duration-300 hover:bg-white hover:border-[#79BFFA]/50 hover:shadow-md">
        <div class="flex h-11 w-11 shrink-0 items-center justify-center rounded-xl bg-[#79BFFA]/15 text-[#2c3e50]">
          <i class="fa-brands fa-linkedin-in text-lg"></i>
        </div>

        <div>
          <span class="block text-[10px] uppercase tracking-widest text-gray-400">
            LinkedIn
          </span>

          <span class="mt-1 block text-sm text-[#2c3e50] group-hover:text-[#79BFFA] transition-colors">
            /cauesousadev
          </span>
        </div>
      </a>

      <!-- GITHUB -->
      <a href="https://github.com/w-Caue" target="_blank" rel="noopener noreferrer"
        class="group flex items-center gap-4 rounded-2xl border border-gray-100 bg-gray-50 p-5 transition-all duration-300 hover:bg-white hover:border-[#79BFFA]/50 hover:shadow-md">
        <div class="flex h-11 w-11 shrink-0 items-center justify-center rounded-xl bg-[#79BFFA]/15 text-[#2c3e50]">
          <i class="fa-brands fa-github text-lg"></i>
        </div>

        <div>
          <span class="block text-[10px] uppercase tracking-widest text-gray-400">
            GitHub
          </span>

          <span class="mt-1 block text-sm text-[#2c3e50] group-hover:text-[#79BFFA] transition-colors">
            /w-Caue
          </span>
        </div>
      </a>

    </div>

    <div class="flex flex-col sm:flex-row items-center justify-between gap-4 mt-8 px-2">
      <p class="text-[10px] uppercase tracking-widest text-gray-400 text-center sm:text-left font-normal">
        Desenvolvedor Full Stack • Java • Spring Boot
      </p>

      <a href="#"
        class="group flex items-center gap-2 text-[10px] uppercase tracking-widest text-gray-400 hover:text-[#79BFFA] transition-colors">
        Voltar ao topo

        <i class="fa-solid fa-arrow-up text-[10px] transition-transform group-hover:-translate-y-1"></i>
      </a>
    </div>
  </section>
</template>

<script setup>
</script>