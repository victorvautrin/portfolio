<script setup>
import { ref } from 'vue'
const props = defineProps(['appName', 'appType'])
const appName = ref(props.appName)

const buttonSrcs = {
  calendar: '/images/calendar_icon.webp',
  mail: '/images/mail.png',
  skills: '/images/competences.png',
  tech: '/images/portable.png'
}

const buttonImageSrc = ref(buttonSrcs[props.appType])

function onAppClick() {
  console.log("L'applicatiion à été cliquée")
}
</script>

<template>
  <div class="appButton">
    <div class="appButton_background" @click="onAppClick">
      <img class="appButton_icon" :src="buttonImageSrc" alt="App Icon" srcset="" />
    </div>
    <span class="appButton_name">{{ appName }}</span>
  </div>
</template>

<style scoped>
.appButton_name {
  font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva,
    Verdana, sans-serif;
  font-weight: bold;
  text-align: center;
  font-size: 0.9rem;
  color: white;
  text-overflow: ellipsis;

  text-shadow: 2px 0px black;
}

.appButton_background {
  width: 7vh;
  height: 7vh;
  background-color: rgb(255, 255, 255);
  border-radius: 1.5vh;
  margin: 0.4vh;
  box-shadow: 2px 2px 0px 1px rgba(0, 0, 0, 0.5);
}

.appButton_background:hover {
  transform: scale(1.03);
}

.appButton_background > img {
  width: 100%;
  height: 100%;
}

.appButton {
  padding: 0vh;
  margin: 2vh;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  border-radius: 1.5vh;
  user-select: none;
}

.appButton_icon {
  width: 80%;
  height: 80%;
}
</style>
