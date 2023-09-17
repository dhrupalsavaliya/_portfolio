<template>
  <v-app-bar :elevation="2">
    <template v-slot:default>
      <div class="ml-3">
        <v-icon v-show="displayIcon" class="bg">mdi-code-json</v-icon>
        <v-icon v-show="!displayIcon" class="bg">mdi-code-brackets</v-icon>
      </div>

      <v-spacer></v-spacer>

      <div class="d-flex justify-center align-center">
        <v-icon>mdi-home</v-icon>
        <a href="#home" class="ml-2" v-if="route === '/'">Home</a>
        <router-link to="/" class="ml-2" v-else>Home</router-link>
      </div>

      <v-spacer></v-spacer>

      <div class="d-flex justify-center align-center">
        <v-icon>mdi-rocket</v-icon>
        <router-link to="/start-up" class="ml-2">SSIP</router-link>
      </div>

      <v-spacer class="contact"></v-spacer>

      <div class="d-flex justify-center align-center blog">
        <v-icon>mdi-post</v-icon>
        <a
          href="https://medium.com/@dhrupalsavaliya09"
          target="_blank"
          class="ml-2"
          >Blog</a
        >
      </div>

      <v-spacer class="contact"></v-spacer>

      <div class="d-flex justify-center align-center contact">
        <v-icon>mdi-human-greeting-proximity</v-icon>
        <a href="#cont" class="ml-2">Contact</a>
      </div>

      <v-spacer></v-spacer>

      <div class="mr-3">
        <v-icon v-show="displayIcon" class="bg"
          >mdi-console-network-outline</v-icon
        >
        <v-icon v-show="!displayIcon" class="bg">mdi-console-network</v-icon>
      </div>
    </template>
  </v-app-bar>
</template>

<script setup>
import { ref } from "vue";
import router from "@/router";

const route = router.currentRoute.value.fullPath;

// console.log(router.currentRoute.value.fullPath);

const displayIcon = ref(true);
setInterval(function () {
  displayIcon.value = !displayIcon.value;
}, 1000);
</script>

<style scoped>
.bg {
  transform: rotateY(45deg);
  animation: rotateAnimation 1s linear infinite;
}

@keyframes rotateAnimation {
  from {
    transform: rotateY(45deg);
  }
  to {
    transform: rotateY(225deg);
  }
}

@media only screen and (max-width: 585px) {
  .blog,
  .contact {
    display: none !important;
  }
}
</style>

