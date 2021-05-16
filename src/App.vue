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
      <v-layout align-center justify-end column class="social-icons">
        <v-btn icon>
          <v-icon> mdi-facebook </v-icon>
        </v-btn>
        <v-btn icon>
          <v-icon> mdi-facebook </v-icon>
        </v-btn>
        <div class="bar" />
      </v-layout>

      <v-layout align-center justify-end column class="email-side">
        <a href="mailto:seanspringmann@comcast.net" class="email-link"
          >seanspringmann@comcast.net</a
        >
        <div class="bar" />
      </v-layout>

      <v-row align="center" class="ma-0" style="height: calc(100vh - 128px)">
        <v-spacer />
        <v-col cols="9">
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

.social-icons {
  position: fixed;
  bottom: 0;
  left: 30px;
}

.email-side {
  position: fixed;
  bottom: 0;
  right: 30px;
}

.email-link {
  writing-mode: vertical-rl;
  padding-right: 90px;
}

.bar {
  height: 90px;
  border-left: 1px solid #d0d0d0;
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
