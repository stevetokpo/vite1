<template>
  <main>
    <section class="h-[30vh] grid place-items-center" id="about-hero-section">
      <h1 class="font-extrabold flex flex-col text-white">
        <span class="text-5xl uppercase">Rencontrez</span>
        <span class="text-6xl pl-12 py-4 font-sacramento flex items-center gap-3"
          >Liquidimmo
          <svg
            xmlns="http://www.w3.org/2000/svg"
            fill="none"
            viewBox="0 0 24 24"
            stroke-width="1.5"
            stroke="currentColor"
            class="w-12 h-12"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              d="m20.25 7.5-.625 10.632a2.25 2.25 0 0 1-2.247 2.118H6.622a2.25 2.25 0 0 1-2.247-2.118L3.75 7.5M10 11.25h4M3.375 7.5h17.25c.621 0 1.125-.504 1.125-1.125v-1.5c0-.621-.504-1.125-1.125-1.125H3.375c-.621 0-1.125.504-1.125 1.125v1.5c0 .621.504 1.125 1.125 1.125Z"
            /></svg
        ></span>
      </h1>
    </section>
    <section class="h-fit px-4 py-5 bg-white">
      <h2 class="font-bold flex flex-col uppercase py-10">
        <span class="text-4xl pl-12 text-gray-900">Rencontrez nos</span
        ><span class="text-4xl text-outline-gray text-white">Fondateurs</span>
      </h2>
      <div class="flex flex-col gap-5">
        <p>
          <b>Liquidimmo</b> est née de l'audace de deux jeunes intrépides. En effet, c'est
          en 2019, Patrick SAAR et Corentin Vasquez ont unis leurs forces pour créer
          l'entreprise qui viendra en aide à des millier de ménages et de structures en
          France.
        </p>
        <p>
          Patrick, expert en <b>Stratégie d'entreprise</b>, apporte sa profonde
          connaissance du secteur, tandis que Conrentin, spécialisé dans
          <b>Développement durable</b>, enrichit l'équipe par son approche innovante.
        </p>
        <div class="flex border-4 border-gray-700 rounded-lg">
          <img src="https://i.imgur.com/z3JkpJ0.png" class="w-1/2" alt="" /><img
            class="w-1/2"
            src="https://i.imgur.com/CZqYQcc.png"
            alt=""
          />
        </div>
        <p>
          Grâce à eux et à leur vision commune pour faire de chaque interaction avec vous
          une expérience exceptionnelle, nous sommes ajourd'hui fière du bout de chemin
          parcouru et de la qualité de nos services.
        </p>
      </div>
    </section>
    <section class="h-fit px-4 py-5 bg-white">
      <h2 class="font-bold flex flex-col uppercase pt-0 pb-10 text-4xl text-gray-900">
        Notre mission
      </h2>
      <div class="flex flex-col gap-5">
        <p>
          Notre mission est de vous libérer du fardeau logistique en utilisant des
          méthodes innovantes. Grâce à une équipe dévouée, nous planifions chaque étape
          avec précision, offrant des interfaces conviviales et des informations complètes
          pour garantir une expérience sans souci.
        </p>
      </div>
    </section>
    <section class="h-fit px-4 py-5">
      <h2 class="font-bold flex flex-col uppercase pt-0 pb-10 text-4xl text-gray-900">
        L'équipe exécutive
      </h2>

      <div id="default-carousel" class="relative w-full" data-carousel="slide">
        <!-- Carousel wrapper -->
        <div class="relative h-64 overflow-hidden rounded-lg md:h-96">
          <!-- Item 1 -->
          <div class="hidden duration-700 ease-in-out" data-carousel-item>
            <div
              class="w-full max-w-sm border border-gray-200 rounded-lg shadow bg-gray-800 dark:border-gray-700"
            >
              <div class="flex flex-col items-center pb-10">
                <img
                  class="w-24 h-24 mb-3 rounded-full shadow-lg"
                  src="https://i.imgur.com/kH2iWFn.jpg"
                  alt="Bonnie image"
                />
                <h5 class="mb-1 text-2xl font-medium text-white">
                  Bonnie Green
                </h5>
                <span class="text-sm text-gray-500 dark:text-gray-400"
                  >Cheffe des opérations</span
                >
              </div>
            </div>
          </div>
          <!-- Item 2 -->
          <div class="hidden duration-700 ease-in-out" data-carousel-item>
            <div
              class="w-full max-w-sm border border-gray-200 rounded-lg shadow bg-gray-800 dark:border-gray-700"
            >
              <div class="flex flex-col items-center pb-10">
                <img
                  class="w-24 h-24 mb-3 rounded-full shadow-lg"
                  src="https://i.imgur.com/kH2iWFn.jpg"
                  alt="Bonnie image"
                />
                <h5 class="mb-1 text-2xl font-medium text-white">
                  Bonnie Green
                </h5>
                <span class="text-sm text-gray-500 dark:text-gray-400"
                  >Cheffe des opérations</span
                >
              </div>
            </div>
          </div>
          <!-- Item 3 -->
          <div class="hidden duration-700 ease-in-out" data-carousel-item>
            <div
              class="w-full max-w-sm border border-gray-200 rounded-lg shadow bg-gray-800 dark:border-gray-700"
            >
              <div class="flex flex-col items-center pb-10">
                <img
                  class="w-24 h-24 mb-3 rounded-full shadow-lg"
                  src="https://i.imgur.com/kH2iWFn.jpg"
                  alt="Bonnie image"
                />
                <h5 class="mb-1 text-2xl font-medium text-white">
                  Bonnie Green
                </h5>
                <span class="text-sm text-gray-500 dark:text-gray-400"
                  >Cheffe des opérations</span
                >
              </div>
            </div>
          </div>
          <!-- Item 4 -->
          <div class="hidden duration-700 ease-in-out" data-carousel-item>
            <div
              class="w-full max-w-sm border border-gray-200 rounded-lg shadow bg-gray-800 dark:border-gray-700"
            >
              <div class="flex flex-col items-center pb-10">
                <img
                  class="w-24 h-24 mb-3 rounded-full shadow-lg"
                  src="https://i.imgur.com/kH2iWFn.jpg"
                  alt="Bonnie image"
                />
                <h5 class="mb-1 text-2xl font-medium text-white">
                  Bonnie Green
                </h5>
                <span class="text-sm text-gray-500 dark:text-gray-400"
                  >Cheffe des opérations</span
                >
              </div>
            </div>
          </div>
          <!-- Item 5 -->
          <div class="hidden duration-700 ease-in-out" data-carousel-item>
            <div
              class="w-full max-w-sm border border-gray-200 rounded-lg shadow bg-gray-800 dark:border-gray-700"
            >
              <div class="flex flex-col items-center pb-10">
                <img
                  class="w-24 h-24 mb-3 rounded-full shadow-lg"
                  src="https://i.imgur.com/kH2iWFn.jpg"
                  alt="Bonnie image"
                />
                <h5 class="mb-1 text-2xl font-medium text-white">
                  Bonnie Green
                </h5>
                <span class="text-sm text-gray-500 dark:text-gray-400"
                  >Cheffe des opérations</span
                >
              </div>
            </div>
          </div>
        </div>
        <!-- Slider indicators -->
        <div
          class="absolute z-30 flex -translate-x-1/2 bottom-5 left-1/2 space-x-3 rtl:space-x-reverse"
        >
          <button
            type="button"
            class="w-3 h-3 rounded-full"
            aria-current="true"
            aria-label="Slide 1"
            data-carousel-slide-to="0"
          ></button>
          <button
            type="button"
            class="w-3 h-3 rounded-full"
            aria-current="false"
            aria-label="Slide 2"
            data-carousel-slide-to="1"
          ></button>
          <button
            type="button"
            class="w-3 h-3 rounded-full"
            aria-current="false"
            aria-label="Slide 3"
            data-carousel-slide-to="2"
          ></button>
          <button
            type="button"
            class="w-3 h-3 rounded-full"
            aria-current="false"
            aria-label="Slide 4"
            data-carousel-slide-to="3"
          ></button>
          <button
            type="button"
            class="w-3 h-3 rounded-full"
            aria-current="false"
            aria-label="Slide 5"
            data-carousel-slide-to="4"
          ></button>
        </div>
        <!-- Slider controls -->
        <button
          type="button"
          class="absolute top-0 start-0 z-30 flex items-center justify-center h-full px-4 cursor-pointer group focus:outline-none"
          data-carousel-prev
        >
          <span
            class="inline-flex items-center justify-center w-10 h-10 rounded-full bg-white/30 dark:bg-gray-800/30 group-hover:bg-white/50 dark:group-hover:bg-gray-800/60 group-focus:ring-4 group-focus:ring-white dark:group-focus:ring-gray-800/70 group-focus:outline-none"
          >
            <svg
              class="w-4 h-4 text-white dark:text-gray-800 rtl:rotate-180"
              aria-hidden="true"
              xmlns="http://www.w3.org/2000/svg"
              fill="none"
              viewBox="0 0 6 10"
            >
              <path
                stroke="currentColor"
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M5 1 1 5l4 4"
              />
            </svg>
            <span class="sr-only">Previous</span>
          </span>
        </button>
        <button
          type="button"
          class="absolute top-0 end-0 z-30 flex items-center justify-center h-full px-4 cursor-pointer group focus:outline-none"
          data-carousel-next
        >
          <span
            class="inline-flex items-center justify-center w-10 h-10 rounded-full bg-white/30 dark:bg-gray-800/30 group-hover:bg-white/50 dark:group-hover:bg-gray-800/60 group-focus:ring-4 group-focus:ring-white dark:group-focus:ring-gray-800/70 group-focus:outline-none"
          >
            <svg
              class="w-4 h-4 text-white dark:text-gray-800 rtl:rotate-180"
              aria-hidden="true"
              xmlns="http://www.w3.org/2000/svg"
              fill="none"
              viewBox="0 0 6 10"
            >
              <path
                stroke="currentColor"
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="m1 9 4-4-4-4"
              />
            </svg>
            <span class="sr-only">Next</span>
          </span>
        </button>
      </div>
    </section>
  </main>
</template>

<script scoped>
import { onMounted } from "vue";
import { initFlowbite } from "flowbite";

onMounted(() => {
  initFlowbite();
});
</script>

<style scoped>
#about-hero-section {
  background: linear-gradient(to bottom, #4a5568, #1a202c);
}
</style>
