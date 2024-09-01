<template>
  <nav class="flex justify-between items-center">
    <div class="">
      <img src="/src/assets/logo.svg" alt="" />
    </div>
    <div v-for="(navLink) in navLinks" :key="navLink.id">
      {{ navLink.label }}
    </div>
     <div class="flex gap-4 items-center">
    <RouterLink to="/login">
    Login</RouterLink>
    <RouterLink class="bg-green-500 p-2 rounded-lg text-white" to="/signup">
    Login</RouterLink>
  </div>
  </nav>
 
</template>

<script setup lang="ts">
import { navLinks } from "../constants/index";
import { RouterLink } from "vue-router";
</script>
