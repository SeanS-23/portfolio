<template>
  <v-app>
    <v-app-bar app dark hide-on-scroll elevation="0" color="#0A182F">
      <v-icon size="32"> mdi-boxing-glove </v-icon>
      <v-spacer />
      <v-btn href="#about" text class="pl-3 pr-3 text-none">
        <span class="text-none teal--text text--accent-1 pr-1"> 01. </span>
        About
      </v-btn>
      <v-btn href="#experience" text class="pl-3 pr-3 text-none">
        <span class="text-none teal--text text--accent-1 pr-1"> 02. </span>
        Experience
      </v-btn>
      <v-btn href="#projects" text class="pl-3 pr-3 text-none">
        <span class="text-none teal--text text--accent-1 pr-1"> 03. </span>
        Projects
      </v-btn>
      <v-btn href="#contact" text class="pl-3 pr-3 text-none">
        <span class="text-none teal--text text--accent-1 pr-1"> 04. </span>
        Contact
      </v-btn>
      <v-btn
        href="./resume.pdf"
        target="_blank"
        color="teal accent-1"
        outlined
        class="pl-3 pr-3 text-none"
      >
        Resume
      </v-btn>
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
        <div class="vertical-bar" />
      </v-layout>

      <v-layout align-center justify-end column class="email-side">
        <a href="mailto:seanspringmann@comcast.net" class="email-link"
          >seanspringmann@comcast.net</a
        >
        <div class="vertical-bar mt-2" />
      </v-layout>

      <v-row justify="center" align="center" class="ma-0">
        <v-col
          cols="12"
          align="center"
          style="max-width: 70rem; padding-left: 5rem; padding-right: 5rem"
        >
          <v-row
            class="ma-0"
            style="height: 100vh"
            justify="center"
            align="center"
          >
            <v-col cols="12" align="start">
              <welcome />
            </v-col>
          </v-row>
          <v-row class="ma-0" justify="center" align="center">
            <v-col cols="12" align="start">
              <a name="about" />
              <about />

              <div style="height: 20rem" />
              <a name="experience" />
              <experience />

              <div style="height: 60rem" />
            </v-col>
          </v-row>
        </v-col>
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
:root .v-application .primary--text {
  color: #a7ffeb !important;
  caret-color: #a7ffeb !important;
}
.main-color {
  color: #d0d0d0;
}
.theme--dark.v-tabs-items {
  background-color: transparent;
}
body::-webkit-scrollbar {
  width: 12px;
}
body::-webkit-scrollbar-track {
  background: #0a182f;
}
body::-webkit-scrollbar-thumb {
  background-color: #4e5681;
  border-radius: 20px;
  margin-right: 5px;
  border: 3px solid #0a182f;
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
.has-anchor {
  padding-top: 6rem;
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
.vertical-bar {
  height: 90px;
  border-left: 1px solid #d0d0d0;
}
.horizontal-bar {
  width: 70%;
  border-top: 1px solid #455a64;
}
.experience-content-container {
  display: flex;
  background-color: transparent;
}
.tab-list {
  position: relative;
  z-index: 3;
  width: max-content;
  padding: 0px;
  margin: 0px;
  list-style: none;
  text-align: left;
}
.company {
  color: #a7ffeb;
}
.tab-textbox {
  width: fit-content;
  height: auto;
}
.tab-content-list {
  list-style: circle;
}
</style>

<script>
import Welcome from "@/components/Welcome.vue";
import About from "@/components/About.vue";
import Experience from "@/components/Experience.vue";
export default {
  name: "App",
  components: { Welcome, About, Experience },
  data: () => ({
    //
  }),
};
</script>
