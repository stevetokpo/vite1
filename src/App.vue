<template>
  <MyHeader />
  <RouterView />
  <MyFooter />
</template>

<script setup>

import { RouterView } from "vue-router";

import MyHeader from "./components/MyHeader.vue";
import MyFooter from "./components/MyFooter.vue";
</script>

