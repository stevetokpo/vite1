<template>
  <section
    ref="section1"
    id="one"
    class="bg-white h-[80vh] md:h-[65vh] lg:h-auto overflow-hidden"
  >
    <div
      ref="title"
      class="text-[2rem] md:text-[4rem] lg:text-[7rem] pt-12 uppercase font-bold leading-none text-gray-700 text-center"
    >
      <span ref="titlePart1" class="block"
        >Votre <span class="text-outline-gray text-transparent">compagnon </span></span
      >
      <span ref="titlePart2" class="block"> de déménagement</span>
    </div>
    <div class="flex flex-col items-center lg:items-start lg:flex-row lg:pt-20 gap-10">
      <div class="px-4 md:px-8 lg:px-24 lg:w-[200vw]">
        <span class="py-8 text-lg md:text-xl block text-[#212121]"
          >Bienvenue chez <span class="font-bold text-black">Liquidimmo</span>, votre
          partenaire de confiance pour tous vos besoins de vide-maison. Nous avons un seul
          objectif; simplifier le processus de débarras de votre propriété. Contactez nous
          dès maintenant et profitez d'une expérience de déménagement sereine et sans
          aucun stress.</span
        >
        <div class="text-gray-700 text-2xl font-bold flex gap-2 items-center">
          <span>Prenez rendez-vous!</span>
          <button>
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
                d="M12.75 15l3-3m0 0l-3-3m3 3h-7.5M21 12a9 9 0 11-18 0 9 9 0 0118 0z"
              />
            </svg>
          </button>
        </div>
      </div>
      <div ref="slidingImage" class="w-[150vw] lg:w-[300vw] lg:translate-x-40 pb-12">
        <img src="https://i.imgur.com/CEX4Rur.png" class="" alt="" />
      </div>
    </div>
  </section>
</template>

<script setup>
import { ref, onMounted } from "vue";
import Lenis from "@studio-freight/lenis";
import { gsap } from "gsap";
import ScrollTrigger from "gsap/ScrollTrigger";

const slidingImage = ref(null);
const title = ref(null);
const titlePart1 = ref(null);
const titlePart2 = ref(null);

const phone = window.matchMedia("(max-width: 600px)");
const tablet = window.matchMedia("(min-width: 600px) and (max-width: 992px)");
const desktop = window.matchMedia("(min-width: 992px)");

onMounted(() => {
  const lenis = new Lenis();

  lenis.on("scroll", (e) => {
    console.log(e);
  });

  function raf(time) {
    lenis.raf(time);
    requestAnimationFrame(raf);
  }

  requestAnimationFrame(raf);

  //gsap scroll trigger part
  gsap.registerPlugin(ScrollTrigger);

  //Phone scrollTrigger animations
  if (phone.matches) {
    gsap.to(titlePart1.value, {
      scrollTrigger: {
        trigger: title.value,
        start: "top 50%",
        end: "bottom top",
        scrub: true,
        markers: false,
      },
      x: 50,
    });

    gsap.to(titlePart2.value, {
      scrollTrigger: {
        trigger: title.value,
        start: "top 50%",
        end: "bottom top",
        scrub: true,
        markers: false,
      },
      x: -50,
    });

    gsap.to(slidingImage.value, {
      scrollTrigger: {
        trigger: slidingImage.value,
        start: "top bottom",
        end: "bottom 10%",
        scrub: true,
        markers: false,
      },
      x: -90,
    });
  }

  //Tablet scrollTrigger animations
  if (tablet.matches) {
    gsap.to(titlePart1.value, {
      scrollTrigger: {
        trigger: title.value,
        start: "top 75%",
        end: "bottom top",
        scrub: true,
        markers: false,
      },
      x: 75,
    });

    gsap.to(titlePart2.value, {
      scrollTrigger: {
        trigger: title.value,
        start: "top 75%",
        end: "bottom top",
        scrub: true,
        markers: false,
      },
      x: -75,
    });

    gsap.to(slidingImage.value, {
      scrollTrigger: {
        trigger: slidingImage.value,
        start: "top bottom",
        end: "bottom 10%",
        scrub: true,
        markers: false,
      },
      x: -150,
    });
  }

  //Desktop scrollTrigger animations

  if (desktop.matches) {
    const timeLine1 = gsap.timeline({
      scrollTrigger: {
        trigger: title.value,
        start: "top bottom",
        end: "top top",
        scrub: true,
        markers: false,
      },
    });

    timeLine1.to(titlePart1.value, { x: "150px" });

    const timeLine2 = gsap.timeline({
      scrollTrigger: {
        trigger: title.value,
        start: "top bottom",
        end: "bottom top",
        scrub: true,
        markers: false,
      },
    });

    timeLine2.to(titlePart2.value, { x: "-150px" });

    const timeline3 = gsap.timeline({
      scrollTrigger: {
        trigger: slidingImage.value,
        start: "top bottom",
        end: "bottom 30%",
        scrub: true,
        markers: false,
      },
    });

    timeline3.to(slidingImage.value, { x: "-10px" });
  }
});
</script>

<style>
#one {
  position: relative;
  z-index: 4;
}
</style>
