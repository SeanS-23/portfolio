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
        <v-btn
          class="social-icon"
          href="https://www.facebook.com/sean.springmann/"
          target="_blank"
          icon
        >
          <v-icon color="#d0d0d0"> mdi-facebook </v-icon>
        </v-btn>
        <v-btn
          class="social-icon"
          href="https://github.com/SeanS-23"
          target="_blank"
          icon
        >
          <v-icon color="#d0d0d0"> mdi-github </v-icon>
        </v-btn>
        <v-btn class="social-icon" icon>
          <v-icon color="#d0d0d0"> mdi-linkedin </v-icon>
        </v-btn>
        <v-btn class="social-icon" icon>
          <v-icon color="#d0d0d0"> mdi-twitch </v-icon>
        </v-btn>
        <v-btn class="social-icon" icon>
          <v-icon color="#d0d0d0"> mdi-youtube </v-icon>
        </v-btn>
        <div class="bar" />
      </v-layout>

      <v-layout align-center justify-end column class="email-side">
        <a href="mailto:seanspringmann@comcast.net" class="email-link"
          >seanspringmann@comcast.net</a
        >
        <div class="bar mt-2" />
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

<style lang="scss">
.body,
html,
body {
  background-color: #0a182f;
}

.social-icons {
  transition: all 0.25s ease;
  position: fixed;
  bottom: 0;
  left: 30px;
}

.social-icon {
  transition: all 0.25s ease;
}

.social-icon:hover {
  i {
    transform: scale(1.05);
    color: #a7ffeb !important;
  }
}

.email-side {
  position: fixed;
  bottom: 0;
  right: 30px;
}

.email-link {
  transition: all 0.25s ease;
  writing-mode: vertical-rl;
  text-decoration: none;
  color: #d0d0d0 !important;
}

.email-link:hover {
  transform: scale(1.05);
  color: #a7ffeb !important;
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
