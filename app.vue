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

<style>
#app {
  font-family: Arial, sans-serif;
}
</style>
