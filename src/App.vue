<script setup lang="ts">
import { RouterLink, RouterView } from "vue-router";
import Navbar from "./components/Navbar.vue";
</script>

<template>
 <main class="p-6">
   <Navbar/>
  <RouterView />
 </main>

</template>
