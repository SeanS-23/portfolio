<template>
  <v-app>
    <v-app-bar app dark hide-on-scroll elevation="0" color="#0A182F">
      <v-spacer />
      <v-btn text class="text-none"> About </v-btn>
      <v-btn text class="text-none"> Experience </v-btn>
      <v-btn text class="text-none"> Work </v-btn>
      <v-btn text class="text-none"> Contact </v-btn>
      <v-btn outlined class="text-none"> Resume </v-btn>
    </v-app-bar>

    <v-main class="body">
      <HelloWorld />
    </v-main>
  </v-app>
</template>

<style>
.body {
  background-color: #0a182f;
}
</style>

<script>
import HelloWorld from "./components/HelloWorld";

export default {
  name: "App",

  components: {
    HelloWorld,
  },

  data: () => ({
    //
  }),
};
</script>
