<template>
  <v-app>
    <v-app-bar app dark hide-on-scroll elevation="0" color="#0A182F">
      <v-icon size="32"> mdi-facebook </v-icon>
      <v-spacer />
      <v-btn text class="text-none"> About </v-btn>
      <v-btn text class="text-none"> Experience </v-btn>
      <v-btn text class="text-none"> Work </v-btn>
      <v-btn text class="text-none"> Contact </v-btn>
      <v-btn color="teal accent-1" outlined class="text-none"> Resume </v-btn>
    </v-app-bar>

    <v-main class="body">
      <v-row>
        <v-spacer />
        <v-col cols="6">
          <welcome />
        </v-col>
        <v-spacer />
      </v-row>
    </v-main>
  </v-app>
</template>

<style>
.body {
  background-color: #0a182f;
}
</style>

<script>
import Welcome from "@/components/Welcome.vue";
export default {
  name: "App",

  components: { Welcome },

  data: () => ({
    //
  }),
};
</script>
