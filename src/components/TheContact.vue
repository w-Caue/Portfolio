<template>
  <section class="font-bold py-3 px-5 mx-2 my-16">
    <div class="grid sm:grid-cols-2 items-center">
      <div>
        <div class="">
          <h1 class="text-3xl">
            Entre em
            <span class="text-[#79BFFA]">contato</span>
          </h1>
        </div>

        <!-- <img
          class="size-72 object-cover rounded-full"
          src="../assets/logo.png"
          alt="modelo"
        /> -->

        <h1 class="text-xl">vamos <span class="text-[#79BFFA]">conversar</span> sobre seu próximo <span class="text-[#79BFFA]">projeto</span>.</h1>
      </div>

      <div class="bg-gray-100 p-5 rounded-lg mt-3">
        <form
          action="https://formsubmit.co/developercaue@gmail.com"
          method="POST"
        >
          <div class="mb-5">
            <label for="name" class="text-start block text-sm text-gray-600">
              Nome *
            </label>
            <input
              type="text"
              name="name"
              id="name"
              required
              class="w-full rounded-t-md border-b border-gray-400 bg-gray-100 p-1 text-sm text-[#6B7280] outline-none focus:bg-white focus:border-blue-500 focus:shadow-md"
            />
          </div>

          <div class="mb-5">
            <label for="email" class="text-start block text-sm text-gray-600">
              Email *
            </label>
            <input
              type="email"
              name="email"
              id="email"
              required
              class="w-full rounded-t-md border-b border-gray-400 bg-gray-100 p-1 text-sm text-[#6B7280] outline-none focus:bg-white focus:border-blue-500 focus:shadow-md"
            />
          </div>

          <div class="mb-5">
            <label for="msg" class="text-start block text-sm text-gray-600">
              Mensagem *
            </label>
            <textarea
              name="msg"
              id="msg"
              rows="1"
              required
              class="w-full rounded-t-md border-b border-gray-400 bg-gray-100 p-1 text-sm text-[#6B7280] outline-none focus:bg-white focus:border-blue-500 focus:shadow-md"
            ></textarea>
          </div>

          <input type="hidden" name="_captcha" value="false" />

          <input
            type="hidden"
            name="_next"
            value="https://caueptfo.netlify.app"
          />

          <button
            class="text-white text-sm bg-[#79BFFA] p-2 rounded-xl cursor-pointer hover:scale-95 transition-all"
          >
            Enviar
          </button>
        </form>
      </div>
    </div>
  </section>
</template>
