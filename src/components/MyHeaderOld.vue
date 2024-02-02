<template>
    <header>
      <div class="flex items-center gap-2 fixed z-40 top-6 md:top-12 left-8 text-white mix-blend-difference">
        <router-link
          to="/"
          class="flex items-center gap-2 fixed top-6 md:top-12 left-8 text-white font-sacramento"
        >
          <h1 class="font-bold text-[2rem] leading-none">Liquidimmo</h1>
          <svg
            xmlns="http://www.w3.org/2000/svg"
            fill="none"
            viewBox="0 0 24 24"
            stroke-width="1.5"
            stroke="currentColor"
            class="w-8 h-8"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              d="m20.25 7.5-.625 10.632a2.25 2.25 0 0 1-2.247 2.118H6.622a2.25 2.25 0 0 1-2.247-2.118L3.75 7.5M10 11.25h4M3.375 7.5h17.25c.621 0 1.125-.504 1.125-1.125v-1.5c0-.621-.504-1.125-1.125-1.125H3.375c-.621 0-1.125.504-1.125 1.125v1.5c0 .621.504 1.125 1.125 1.125Z"
            />
          </svg>
        </router-link>
        <button
          type="button"
          data-drawer-target="drawer-right-example"
          data-drawer-show="drawer-right-example"
          data-drawer-placement="right"
          aria-controls="drawer-right-example"
        >
          <svg
            xmlns="http://www.w3.org/2000/svg"
            fill="none"
            viewBox="0 0 24 24"
            stroke-width="1.5"
            stroke="currentColor"
            class="w-8 md:w-10 h-8 md:h-10 fixed z-10 top-6 md:top-12 right-8 text-white hover:lg:text-gray-900"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              d="M3.75 6.75h16.5M3.75 12h16.5m-16.5 5.25h16.5"
            />
          </svg>
        </button>
      </div>
      <!-- drawer component -->
      <div
        id="drawer-right-example"
        class="fixed top-0 right-0 z-40 h-screen p-4 overflow-y-auto transition-transform translate-x-full bg-white w-80"
        tabindex="-1"
        aria-labelledby="drawer-right-label"
      >
        <h5
          id="drawer-right-label"
          class="text-base font-semibold text-gray-700 uppercase dark:text-gray-400"
        >
          Menu
        </h5>
        <button
          type="button"
          data-drawer-hide="drawer-right-example"
          aria-controls="drawer-right-example"
          class="text-gray-400 bg-transparent hover:bg-gray-200 hover:text-gray-900 rounded-lg text-sm w-8 h-8 absolute top-2.5 end-2.5 inline-flex items-center justify-center dark:hover:bg-gray-600 dark:hover:text-white"
        >
          <svg
            class="w-3 h-3"
            aria-hidden="true"
            xmlns="http://www.w3.org/2000/svg"
            fill="none"
            viewBox="0 0 14 14"
          >
            <path
              stroke="currentColor"
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="m1 1 6 6m0 0 6 6M7 7l6-6M7 7l-6 6"
            />
          </svg>
          <span class="sr-only">Close menu</span>
        </button>
        <div class="py-4 overflow-y-auto">
          <ul class="space-y-2 font-medium">
            <li>
              <router-link
                to="/"
                data-drawer-hide="drawer-right-example"
                aria-controls="drawer-right-example"
                class="flex items-center p-2 text-gray-700 rounded-lg hover:bg-gray-100 group"
              >
                <svg
                  class="w-5 h-5 text-gray-500 transition duration-75 dark:text-gray-400 group-hover:text-gray-900 dark:group-hover:text-white"
                  xmlns="http://www.w3.org/2000/svg"
                  viewBox="0 0 576 512"
                >
                  <!--!Font Awesome Free 6.5.1 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free Copyright 2024 Fonticons, Inc.-->
                  <path
                    d="M575.8 255.5c0 18-15 32.1-32 32.1h-32l.7 160.2c0 2.7-.2 5.4-.5 8.1V472c0 22.1-17.9 40-40 40H456c-1.1 0-2.2 0-3.3-.1c-1.4 .1-2.8 .1-4.2 .1H416 392c-22.1 0-40-17.9-40-40V448 384c0-17.7-14.3-32-32-32H256c-17.7 0-32 14.3-32 32v64 24c0 22.1-17.9 40-40 40H160 128.1c-1.5 0-3-.1-4.5-.2c-1.2 .1-2.4 .2-3.6 .2H104c-22.1 0-40-17.9-40-40V360c0-.9 0-1.9 .1-2.8V287.6H32c-18 0-32-14-32-32.1c0-9 3-17 10-24L266.4 8c7-7 15-8 22-8s15 2 21 7L564.8 231.5c8 7 12 15 11 24z"
                  />
                </svg>
                <span class="ms-3 hover:text-gray-900">Accueil</span>
              </router-link>
            </li>
            <li>
              <a
                class="flex items-center p-2 text-gray-700 rounded-lg hover:bg-gray-100 group"
              >
                <svg
                  class="w-5 h-5 text-gray-500 transition duration-75 dark:text-gray-400 group-hover:text-gray-900 dark:group-hover:text-white"
                  xmlns="http://www.w3.org/2000/svg"
                  viewBox="0 0 448 512"
                >
                  <!--!Font Awesome Free 6.5.1 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free Copyright 2024 Fonticons, Inc.-->
                  <path
                    d="M427.8 380.7l-196.5 97.8a18.6 18.6 0 0 1 -14.7 0L20.2 380.7c-4-2-4-5.3 0-7.3L67.2 350a18.7 18.7 0 0 1 14.7 0l134.8 67a18.5 18.5 0 0 0 14.7 0l134.8-67a18.6 18.6 0 0 1 14.7 0l47.1 23.4c4.1 2 4.1 5.2 0 7.2zm0-136.5l-47.1-23.4a18.6 18.6 0 0 0 -14.7 0l-134.8 67.1a18.7 18.7 0 0 1 -14.7 0L81.9 220.7a18.7 18.7 0 0 0 -14.7 0l-47.1 23.4c-4 2-4 5.3 0 7.3l196.5 97.8a18.6 18.6 0 0 0 14.7 0l196.5-97.8c4.1-2 4.1-5.3 0-7.3zM20.2 130.4l196.5 90.3a20.1 20.1 0 0 0 14.7 0l196.5-90.3c4-1.9 4-4.9 0-6.7L231.3 33.4a19.9 19.9 0 0 0 -14.7 0l-196.5 90.3c-4.1 1.9-4.1 4.9 0 6.7z"
                  />
                </svg>
                <span class="ms-3 hover:text-gray-900">Nos services</span>
              </a>
            </li>
            <li>
              <router-link
                to="/about"
                class="flex items-center p-2 text-gray-700 rounded-lg hover:bg-gray-100 group"
              >
                <svg
                  class="w-5 h-5 text-gray-500 transition duration-75 dark:text-gray-400 group-hover:text-gray-900 dark:group-hover:text-white"
                  xmlns="http://www.w3.org/2000/svg"
                  viewBox="0 0 512 512"
                >
                  <!--!Font Awesome Free 6.5.1 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free Copyright 2024 Fonticons, Inc.-->
                  <path
                    d="M256 512A256 256 0 1 0 256 0a256 256 0 1 0 0 512zM216 336h24V272H216c-13.3 0-24-10.7-24-24s10.7-24 24-24h48c13.3 0 24 10.7 24 24v88h8c13.3 0 24 10.7 24 24s-10.7 24-24 24H216c-13.3 0-24-10.7-24-24s10.7-24 24-24zm40-208a32 32 0 1 1 0 64 32 32 0 1 1 0-64z"
                  />
                </svg>
                <span class="ms-3 hover:text-gray-900">À propos</span>
              </router-link>
            </li>
            <li>
              <router-link
                to="/contact"
                data-drawer-hide="drawer-right-example"
                aria-controls="drawer-right-example"
                class="flex items-center p-2 text-gray-700 rounded-lg hover:bg-gray-100 group"
              >
                <svg
                  class="w-5 h-5 text-gray-500 transition duration-75 dark:text-gray-400 group-hover:text-gray-900 dark:group-hover:text-white"
                  xmlns="http://www.w3.org/2000/svg"
                  viewBox="0 0 512 512"
                >
                  <!--!Font Awesome Free 6.5.1 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free Copyright 2024 Fonticons, Inc.-->
                  <path
                    d="M64 0C28.7 0 0 28.7 0 64V352c0 35.3 28.7 64 64 64h96v80c0 6.1 3.4 11.6 8.8 14.3s11.9 2.1 16.8-1.5L309.3 416H448c35.3 0 64-28.7 64-64V64c0-35.3-28.7-64-64-64H64z"
                  />
                </svg>
                <span class="ms-3 hover:text-gray-900">Contact</span>
              </router-link>
            </li>
          </ul>
        </div>
      </div>
    </header>
  </template>
  
  <script setup>
  import { RouterLink } from "vue-router";
  import { onMounted } from "vue";
  import { initFlowbite } from "flowbite";
  
  onMounted(() => {
    initFlowbite();
  });
  </script>
  