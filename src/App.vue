<template>
  <v-app>
    <v-app-bar app dark hide-on-scroll elevation="0" color="#0A182F">
      <v-toolbar-items>
        <v-btn class="text-none"> About </v-btn>
        <v-btn class="text-none"> Experience </v-btn>
        <v-btn class="text-none"> Work </v-btn>
        <v-btn class="text-none"> Contact </v-btn>
        <v-btn class="text-none"> Resume </v-btn>
      </v-toolbar-items>
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
