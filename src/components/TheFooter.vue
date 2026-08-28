<template>
  <footer class="border-t border-gray-100 bg-white">
    <div class="container mx-auto px-5">

      <div class="flex flex-col md:flex-row items-center justify-between gap-6 py-8">

        <a href="#" class="group inline-flex items-center gap-3">
          <span class="relative text-xl font-bold flex items-center justify-center w-10 h-10 rounded-lg
           bg-[#2c3e50] text-[#79BFFA]
           overflow-hidden
           group-hover:bg-[#79BFFA]
           group-hover:text-[#2c3e50]
           transition-all duration-300">
            C
          </span>

          <span class="flex flex-col text-start leading-none">
            <span class="text-xl font-bold uppercase text-[#2c3e50]">
              Cauê Sousa <span class="text-[#79BFFA]">.</span>
            </span>

            <span class="mt-1 text-[8px] uppercase tracking-[0.3em] text-gray-400 font-medium">
              Software Developer
            </span>
          </span>
        </a>

        <nav>
          <ul class="flex flex-wrap items-center justify-center gap-5 sm:gap-7">
            <li>
              <a href="#about"
                class="text-xs uppercase tracking-widest text-gray-500 hover:text-[#79BFFA] transition-colors">
                Sobre
              </a>
            </li>

            <li>
              <a href="#skills"
                class="text-xs uppercase tracking-widest text-gray-500 hover:text-[#79BFFA] transition-colors">
                Skills
              </a>
            </li>

            <li>
              <a href="#project"
                class="text-xs uppercase tracking-widest text-gray-500 hover:text-[#79BFFA] transition-colors">
                Projetos
              </a>
            </li>

            <li>
              <a href="#contact"
                class="text-xs uppercase tracking-widest text-gray-500 hover:text-[#79BFFA] transition-colors">
                Contato
              </a>
            </li>
          </ul>
        </nav>

        <div class="flex items-center gap-2">

          <a href="https://github.com/w-Caue" target="_blank" rel="noopener noreferrer" aria-label="GitHub"
            class="flex items-center justify-center w-9 h-9 rounded-full border border-gray-200 text-[#2c3e50] hover:bg-[#2c3e50] hover:text-white hover:border-[#2c3e50] transition-all duration-300">
            <i class="fa-brands fa-github text-sm"></i>
          </a>

          <a href="https://www.linkedin.com/in/cauesousadev/" target="_blank" rel="noopener noreferrer"
            aria-label="LinkedIn"
            class="flex items-center justify-center w-9 h-9 rounded-full border border-gray-200 text-[#2c3e50] hover:bg-[#2c3e50] hover:text-white hover:border-[#2c3e50] transition-all duration-300">
            <i class="fa-brands fa-linkedin-in text-sm"></i>
          </a>

          <a href="mailto:developercaue@email.com" aria-label="E-mail"
            class="flex items-center justify-center w-9 h-9 rounded-full border border-gray-200 text-[#2c3e50] hover:bg-[#79BFFA] hover:border-[#79BFFA] transition-all duration-300">
            <i class="fa-solid fa-envelope text-sm"></i>
          </a>

        </div>
      </div>

      <div class="h-px bg-gray-100"></div>

      <div class="flex flex-col sm:flex-row items-center justify-between gap-3 py-5">

        <p class="text-[10px] uppercase tracking-widest text-gray-400 font-normal text-center sm:text-left">
          © {{ new Date().getFullYear() }} Cauê Sousa. Todos os direitos reservados.
        </p>

        <div class="flex items-center gap-2">
          <span class="text-[10px] uppercase tracking-widest text-gray-400 font-normal">
            Desenvolvido com
          </span>

          <i class="devicon-vuejs-plain colored text-sm"></i>

          <span class="text-[10px] uppercase tracking-widest text-gray-400 font-normal">
            Vue.js
          </span>
        </div>

      </div>

    </div>
  </footer>
</template>

<script setup>
</script>