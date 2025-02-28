<template>
  <div id="app">
    <NuxtLayout>
      <NuxtPage />
    </NuxtLayout>
  </div>
</template>

<script lang="ts">
import NavbarComponent from "@/components/Navbar/index.vue";
import HomeComponent from "~/components/Home/index.vue";

export default {
  name: "App",
  components: {
    NavbarComponent,
    HomeComponent,
  },
};
</script>

<script setup lang="ts">
import '@fortawesome/fontawesome-svg-core/styles.css'

useHead({
  title: "Claudio Rojas Alarcon | CEO Mondano - Asesor",
  meta: [
    {
      name: "viewport",
      content: "width=device-width, initial-scale=1, maximum-scale=1, user-scalable=no",
    },
    {
      name: "description",
      content:
        "CEO y Co-Founder de Mondano.cl, asesor empresarial especializado en moda y estrategia de negocios en Chile.",
    },
    { property: "og:title", content: "Claudio Rojas | CEO Mondano - Asesor Empresarial" },
    { property: "og:description", content: "Esta es mi marca personal, dejame contarte de que va" },
    { property: "og:image", content: "https://www.claudiorojasalarcon.cl/claudio-pic.jpeg" },
    { property: "og:image:secure_url", content: "https://www.claudiorojasalarcon.cl/claudio-pic.jpeg" },
    { property: "og:image:type", content: "image/jpeg" },
    { property: "og:image:width", content: "300" },
    { property: "og:image:height", content: "300" },
    { property: "og:image:alt", content: "Claudio Rojas Alarcon" },
    { property: "og:type", content: "website" },
    { property: "og:url", content: "https://www.claudiorojasalarcon.cl" },
    { name: "twitter:card", content: "summary_large_image" },
    { name: "twitter:image", content: "https://www.claudiorojasalarcon.cl/claudio-pic.jpeg" },
    { name: "keywords", content: "Claudio Rojas Alarcón, marca personal, mondano, moda" },
    {
      name: "og:site_name",
      content: "Claudio Rojas Alarcon",
    },
    {
      name: "og:locale",
      content: "es_CL",
    },
  ],
  link: [
    { rel: "canonical", href: "https://www.claudiorojasalarcon.cl" },
    { rel: "icon", type: "image/x-icon", href: "https://www.claudiorojasalarcon.cl/favicon.ico" },
    // Apple Touch Icons
    { rel: "apple-touch-icon", sizes: "180x180", href: "/apple-touch-icon.png" },
    { rel: "apple-touch-icon", sizes: "152x152", href: "/apple-touch-icon-152x152.png" },
    { rel: "apple-touch-icon", sizes: "120x120", href: "/apple-touch-icon-120x120.png" },
    { rel: "apple-touch-icon", sizes: "76x76", href: "/apple-touch-icon-76x76.png" },
    { rel: "manifest", href: "/manifest.json" },
  ],
});
</script>

<style>
#app {
  font-family: Arial, sans-serif;
}
</style>
