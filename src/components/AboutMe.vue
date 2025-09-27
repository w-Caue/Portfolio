<template>
  <section class="font-bold py-3 px-5 mx-2 sm:mx-32 my-16 bg-gray-100 rounded-xl">
    <div class="text-start">
      <h1 class="text-3xl">Sobre <span class="text-[#79BFFA]">mim</span></h1>

      <p class="mt-5">
        Sou desenvolvedor com experiência no desenvolvimento de aplicações web
        modernas e escaláveis, atuando tanto no
        <span class="text-[#79BFFA]">frontend</span> quanto no
        <span class="text-[#79BFFA]">backend</span>. Possuo sólida base em
        <span class="text-[#79BFFA]">JavaScript</span>,
        <span class="text-[#79BFFA]">PHP</span> e
        <span class="text-[#79BFFA]">Java</span>, além de frameworks e
        ferramentas que aceleram a
        <span class="text-[#79BFFA]">criação</span> de soluções completas e bem
        <span class="text-[#79BFFA]">estruturadas</span>.
      </p>
    </div>

    <div class="text-start mt-5 grid sm:grid-cols-2 gap-5">
      <div>
        <h1 class="text-xl">
          <span class="text-[#79BFFA]">Dados</span> Pessoais
        </h1>
        <ul class="mt-2">
          <li>
            <h1 class="">
              Telefone:
              <span class="text-[#79BFFA]">85 9 8165 5691</span>
            </h1>
          </li>
          <li>
            <h1 class="">
              Email:
              <span class="text-[#79BFFA]">developercaue@gmail.com</span>
            </h1>
          </li>
          <li>
            <h1 class="">
              Data Nasc.:
              <span class="text-[#79BFFA]">07/10/2002</span>
            </h1>
          </li>
          <li>
            <h1 class="">
              Localização:
              <span class="text-[#79BFFA]">Presidente Kennedy - Fortaleza</span>
            </h1>
          </li>
        </ul>
      </div>
      <div>
        <h1 class="text-xl">
          Meus
          <span class="text-[#79BFFA]">Interesses</span>
        </h1>
        <div class="flex flex-wrap gap-5 text-white mt-2">
          <button
            class="flex flex-col items-center bg-[#79BFFA] p-2 text-center rounded-lg"
          >
            <svg
              xmlns="http://www.w3.org/2000/svg"
              viewBox="0 0 24 24"
              fill="none"
              stroke="currentColor"
              stroke-width="2"
              stroke-linecap="round"
              stroke-linejoin="round"
              class="size-7 lucide lucide-gamepad2-icon lucide-gamepad-2"
            >
              <line x1="6" x2="10" y1="11" y2="11" />
              <line x1="8" x2="8" y1="9" y2="13" />
              <line x1="15" x2="15.01" y1="12" y2="12" />
              <line x1="18" x2="18.01" y1="10" y2="10" />
              <path
                d="M17.32 5H6.68a4 4 0 0 0-3.978 3.59c-.006.052-.01.101-.017.152C2.604 9.416 2 14.456 2 16a3 3 0 0 0 3 3c1 0 1.5-.5 2-1l1.414-1.414A2 2 0 0 1 9.828 16h4.344a2 2 0 0 1 1.414.586L17 18c.5.5 1 1 2 1a3 3 0 0 0 3-3c0-1.545-.604-6.584-.685-7.258-.007-.05-.011-.1-.017-.151A4 4 0 0 0 17.32 5z"
              />
            </svg>
            <span class="text-sm">Games</span>
          </button>

          <button
            class="flex flex-col items-center bg-[#79BFFA] p-2 rounded-lg"
          >
            <svg
              xmlns="http://www.w3.org/2000/svg"
              viewBox="0 0 24 24"
              fill="none"
              stroke="currentColor"
              stroke-width="2"
              stroke-linecap="round"
              stroke-linejoin="round"
              class="size-7 lucide lucide-headphones-icon lucide-headphones"
            >
              <path
                d="M3 14h3a2 2 0 0 1 2 2v3a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-7a9 9 0 0 1 18 0v7a2 2 0 0 1-2 2h-1a2 2 0 0 1-2-2v-3a2 2 0 0 1 2-2h3"
              />
            </svg>
            <span class="text-sm">Music</span>
          </button>

          <button
            class="flex flex-col items-center bg-[#79BFFA] p-2 rounded-lg"
          >
            <svg
              xmlns="http://www.w3.org/2000/svg"
              viewBox="0 0 24 24"
              fill="none"
              stroke="currentColor"
              stroke-width="2"
              stroke-linecap="round"
              stroke-linejoin="round"
              class="size-7 lucide lucide-clapperboard-icon lucide-clapperboard"
            >
              <path
                d="M20.2 6 3 11l-.9-2.4c-.3-1.1.3-2.2 1.3-2.5l13.5-4c1.1-.3 2.2.3 2.5 1.3Z"
              />
              <path d="m6.2 5.3 3.1 3.9" />
              <path d="m12.4 3.4 3.1 4" />
              <path d="M3 11h18v8a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2Z" />
            </svg>
            <span class="text-sm">Cinema</span>
          </button>

          <button
            class="flex flex-col items-center bg-[#79BFFA] p-2 rounded-lg"
          >
            <svg
              xmlns="http://www.w3.org/2000/svg"
              viewBox="0 0 64 64"
              class="size-8"
              fill="none"
              stroke="currentColor"
              stroke-width="3"
            >
              <!-- Faixa horizontal -->
              <rect x="2" y="24" width="60" height="8" rx="2" ry="2" />
              <!-- Nó do cinturão -->
              <rect
                x="26"
                y="20"
                width="12"
                height="16"
                rx="2"
                ry="2"
                fill="currentColor"
              />
              <!-- Ponta esquerda -->
              <rect x="20" y="36" width="6" height="18" rx="2" ry="2" />
              <!-- Ponta direita -->
              <rect x="38" y="36" width="6" height="18" rx="2" ry="2" />
            </svg>

            <span class="text-sm">Jiu-Jitsu</span>
          </button>
        </div>
      </div>
    </div>
  </section>
</template>
