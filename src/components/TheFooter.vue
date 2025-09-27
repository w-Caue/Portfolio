<template>
  <footer>
    <div class="px-4 pt-16 bg-gray-100 md:px-24 lg:px-8">
      <div class="grid gap-10 row-gap-6 mb-8 sm:grid-cols-2 lg:grid-cols-4">
        <div class="sm:col-span-2 flex flex-col justify-start">
          <a
            href="/"
            aria-label="Go home"
            title="Company"
            class="inline-flex items-center"
          >
            <img class="w-22 rounded-lg" src="../assets/logo.png" alt="logo" />
          </a>
        </div>
        <div class="space-y-2 font-bold">
          <p class="text-start">Contato</p>

          <div class="flex text-sm">
            <p class="mr-1 text-gray-800">Email:</p>
            <a
              href="mailto:developercaue@gmail.com"
              aria-label="Our email"
              title="Our email"
              class="transition-colors duration-300 text-deep-purple-accent-400 hover:text-deep-purple-800"
              >developercaue@gmail.com</a
            >
          </div>
        </div>
        <div>
          <p class="text-start font-bold">Social</p>
          <div class="flex space-x-3">
            <button
              onclick="window.open('https://www.instagram.com/caue_dev?igsh=NjJpMTBrM2xvZ2Vu', '_blank')"
              class="text-gray-600 p-2 cursor-pointer hover:bg-gray-200 rounded-full hover:scale-95 transition-all"
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
                class="lucide lucide-instagram-icon lucide-instagram"
              >
                <rect width="20" height="20" x="2" y="2" rx="5" ry="5" />
                <path d="M16 11.37A4 4 0 1 1 12.63 8 4 4 0 0 1 16 11.37z" />
                <line x1="17.5" x2="17.51" y1="6.5" y2="6.5" />
              </svg>
            </button>

            <button
              onclick="window.open('https://github.com/w-Caue', '_blank')"
              class="text-gray-600 p-2 cursor-pointer hover:bg-gray-200 rounded-full hover:scale-95 transition-all"
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
            </button>

            <button
              onclick="window.open('https://www.linkedin.com/in/w-cauedev/', '_blank')"
              class="text-gray-600 p-2 cursor-pointer hover:bg-gray-200 rounded-full hover:scale-95 transition-all"
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
            </button>
          </div>
        </div>
      </div>
      <div
        class="flex flex-col-reverse justify-between pt-5 pb-10 border-t border-gray-200 lg:flex-row"
      >
        <p class="text-sm text-gray-600 font-bold">© Copyright 2025</p>
      </div>
    </div>
  </footer>
</template>
