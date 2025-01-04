<template>
  <div id="app">
    <NavbarComponent />
    <HomeComponent />
    <router-view />
  </div>
</template>

<script lang="ts">
import NavbarComponent from "@/components/Navbar/index.vue";
import HomeComponent from "@/components/Home/index.vue";

export default {
  name: "App",
  components: {
    NavbarComponent,
    HomeComponent,
  },
};
</script>

<script setup lang="ts">
useHead({
  title: "Claudio Rojas Alarcon",
  meta: [{ name: "description", content: "Marca personal de Claudio Rojas Alarcon" }],
});
useSeoMeta({
  title: "Claudio Rojas Alarcon",
  description: "Marca personal de Claudio Rojas Alarcon",
  ogTitle: "Claudio Rojas Alarcon",
  ogDescription: "Esta es mi marca personal, dejame contarte de que va",
  ogImage: "@/assets/claudio-pic.jpeg",
  ogType: "website",
  ogUrl: "https://claudiorojasalarcon.com",
  twitterCard: "summary_large_image",
});
</script>

<style>
#app {
  font-family: Arial, sans-serif;
}
</style>
