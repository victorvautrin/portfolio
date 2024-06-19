<script setup>
import BottomCommands from './components/BottomCommands.vue'
import { RouterView } from 'vue-router'
import PhoneTop from './components/PhoneTop.vue'
////
console.log('Portfolio App started!')
</script>

<template>
  <!-- LINKS FOR ROUTER -->

  <!--
  <RouterLink to="/">Home</RouterLink>
  <RouterLink to="/about">About</RouterLink>
  <RouterView />
  -->
  <div id="phone">
    <div id="phoneScreen">
      <PhoneTop />
      <main>
        <RouterView />
      </main>
      <!-- SHIT KEEPS BREAKING EVERYTHING
        <BottomCommands id="bottomCommands" /> 
        -->
    </div>
  </div>
</template>

<style scoped>
body main {
  height: calc(100% - (1rem + 0.5vh));
  overflow-y: auto;
}

#phoneScreen {
  background-image: url('public/images/phone_wallpaper.webp');
  background-size: cover;
}

@media (max-width: 480px) {
  #phoneScreen {
    background-color: rgb(184, 125, 36);
    width: 100vw;
    height: 100vh;
  }

  main {
    height: 100%;
  }

  #bottomCommands {
    display: none;
  }
}

@media (min-width: 481px) {
  #phone {
    background-color: black;
    width: fit-content;
    padding: 2vh;
    border-radius: 2vh;
    z-index: 20;
  }

  #phoneScreen {
    background-color: rgb(184, 125, 36);
    width: 40vh;
    height: 80vh;
  }
}
/* HEIGHT */
/* HEIGHT */
/* HEIGHT */
</style>
