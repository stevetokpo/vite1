<template>
    <div data-animation="default" data-collapse="all" data-duration="400" data-easing="ease" data-easing2="ease" role="banner" class="navbar-section w-nav">
        <div class="navbar-wrapper">
            <span class="navbar-logo w-nav-brand w--current">
                <router-link to="/" class="flex items-center gap-2 fixed top-6 left-8 text-white font-sacramento">
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
            </span>
            <div data-w-id="88b6df5b-dbac-87c1-0eb9-7f67953d09e7" class="navbar-menu-button w-nav-button">
                <img src="/open.svg" loading="lazy" alt="" class="navbar-menu-open ton" @click="switchoc(1)"/>
                <img src="/close.svg" loading="lazy" alt="" class="navbar-menu-close toff" @click="switchoc(0)"/>
            </div>
        </div>
        <nav role="navigation" class="navbar-menu w-nav-menu">
            <div class="navbar-menu-wrapper">
                <router-link to="#hero" aria-current="page" class="navbar-link w-inline-block w--current"  @click="closemenu()">
                    <h4 class="navbar-link-text">
                        Accueil
                    </h4>
                </router-link>
                <router-link to="#two" class="navbar-link w-inline-block" @click="closemenu()">
                    <h4 class="navbar-link-text">
                        À propos
                    </h4>
                </router-link>
                <router-link to="#four" class="navbar-link w-inline-block" @click="closemenu()">
                    <h4 class="navbar-link-text">
                        Nos services
                    </h4>
                </router-link>
                <router-link to="#footer" class="navbar-link w-inline-block" @click="closemenu()">
                    <h4 class="navbar-link-text">Contact</h4>
                </router-link>
            </div>
        </nav>
    </div>
</template>

<script setup>
    import { RouterLink } from "vue-router";
    import { onMounted } from "vue";
    import { initFlowbite } from "flowbite";

    onMounted(() => {
        initFlowbite();
    });
    function switchoc(orc) {
        const openIcons = document.querySelectorAll('.ton');
        const closeIcons = document.querySelectorAll('.toff');

        if (orc) {
            openIcons.forEach(icon => icon.style.display = "none");
            closeIcons.forEach(icon => icon.style.display = "inline-block");
        }
        else {
            openIcons.forEach(icon => icon.style.display = "inline-block");
            closeIcons.forEach(icon => icon.style.display = "none");
        }
    }
    function closemenu() {
        const openIcon = document.querySelector('.navbar-menu-open.ton');
        if (openIcon) {
            openIcon.click();
            switchoc(0)
        }
    }
</script>