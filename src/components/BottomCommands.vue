<script setup>
import { RouterLink } from 'vue-router'
</script>

<template>
  <div class="phoneCommands">
    <RouterLink class="RouterLinkClass bottomCommandItem" to="/">⚪</RouterLink>
  </div>
</template>

<style scoped>
.bottomCommandItem {
  padding: 0.8vh;
}

.RouterLinkClass {
  text-decoration: none;
}

.phoneCommands {
  font-size: 1.5rem;
  position: relative;
  width: 100%;
  display: flex;
  justify-content: space-around;
  background-color: rgba(0, 0, 0, 1);
  color: white;
  font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
}

.phoneCommands > span {
  padding: 10px;
}
</style>
