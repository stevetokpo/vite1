<template>
  <footer id="footer" class="lg:h-[120vh] bg-white lg:bg-gray-900 w-screen">
    <section class="lg:h-screen relative">
      <div class="lg:pt-32 lg:pl-80 flex flex-col items-center lg:flex-row">
        <div
          class="lg:h-[300px] text-gray-900 lg:text-white relative w-fit flex flex-col lg:block"
        >
          <h2
            class="text-[2rem] md:text-[3.5rem] lg:text-[6rem] mt-24 lg:mt-0 py-8 lg:py-0 font-bold leading-none font-manrope"
          >
            Notre équipe <br />
            <span class="hidden lg:inline">&emsp;</span>vous attends
          </h2>
          <router-link
            to="/contact"
            class="lg:hover:scale-125 transition-all lg:hover:text-white"
          >
            <button
              class="font-bold w-fit mx-auto lg:mx-0 text-xl lg:absolute lg:bottom-0 lg:right-32 p-3 rounded-full bg-gray-900 text-white hover:lg:bg-white hover:lg:scale-105 hover:lg:text-gray-900 transition-all contact-us-button"
            >
              Contactez-nous
            </button>
          </router-link>
        </div>
        <img
          src="https://i.imgur.com/triCJmR.png"
          class="mt-32 w-full lg:w-[28%] lg:absolute lg:bottom-0 lg:left-0"
          alt=""
        />
        <div
          class="text-white text-xl md:text-2xl lg:text-xl font-semibold py-12 md:py-16 lg:py-0 md:pl-16 :pl-28 lg:pt-10 w-full lg:w-auto bg-gray-900 lg:bg-none"
        >
          <div class="w-[75%] md:w-auto lg:w-[300px] mx-auto flex flex-col gap-5">
            <span class="text-[1.5rem] md:text-[2rem] lg:text-[1.5rem]">Menu</span>
            <div
              class="h-[75px] text-gray-400 flex justify-between md:justify-normal lg:justify-between md:gap-20"
            >
              <div class="flex flex-col justify-between">
                <router-link
                  to="/"
                  class="lg:hover:scale-125 transition-all lg:hover:text-white"
                  >Accueil</router-link
                ><a href="" class="lg:hover:scale-125 transition-all lg:hover:text-white"
                  >Nos services</a
                >
              </div>
              <div class="flex flex-col justify-between">
                <router-link to="/about" class="lg:hover:scale-125 transition-all lg:hover:text-white"
                  >À propos</router-link
                >
                <router-link
                  to="/contact"
                  class="lg:hover:scale-125 transition-all lg:hover:text-white"
                  >Contact</router-link
                >
              </div>
            </div>
          </div>
          <div
            class="flex gap-8 text-gray-900 justify-center md:justify-normal py-10 cursor-pointer"
          >
            <div
              class="bg-white rounded-full h-8 w-8 md:h-10 md:w-10 flex justify-center items-center lg:hover:scale-125 transition-all"
            >
              <i class="fa-brands fa-facebook-f"></i>
            </div>
            <div
              class="bg-white rounded-full h-8 w-8 md:h-10 md:w-10 flex justify-center items-center lg:hover:scale-125 transition-all"
            >
              <i class="fa-brands fa-tiktok"></i>
            </div>
            <div
              class="bg-white rounded-full h-8 w-8 md:h-10 md:w-10 flex justify-center items-center lg:hover:scale-125 transition-all"
            >
              <i class="fa-brands fa-instagram"></i>
            </div>
            <div
              class="bg-white rounded-full h-8 w-8 md:h-10 md:w-10 flex justify-center items-center lg:hover:scale-125 transition-all"
            >
              <i class="fa-brands fa-linkedin-in"></i>
            </div>
          </div>
        </div>
      </div>
    </section>
    <div class="border-t-2 h-32 p-12 lg:h-auto border-t-gray-400 relative bg-gray-900">
      <span class="text-gray-400 font-semibold lg:absolute lg:top-16 lg:right-40"
        >Created by <span class="text-white font-bold">People</span></span
      >
    </div>
  </footer>
</template>

<script setup>
import { RouterLink } from "vue-router";
import "@fortawesome/fontawesome-free/css/all.css";
import ContactPageView from "@/views/ContactPageView.vue";
</script>
