<script setup>
import AppButton from '/src/components/AppButton.vue'
import { RouterLink } from 'vue-router'
</script>

<template>
  <div class="appsContainer">
    <!-- CONTACT -->
    <RouterLink class="AppButtonLink" to="/contact">
      <AppButton appType="mail" appName="Contact" />
    </RouterLink>
    <!-- CONTACT -->
    <RouterLink class="AppButtonLink" to="/competences">
      <AppButton appType="tech" appName="Technologies" />
    </RouterLink>

    <RouterLink class="AppButtonLink" to="/portefeuillecompetences">
      <AppButton appType="skills" appName="Portefeuille de Compétences" />
    </RouterLink>
  </div>
</template>

<style scoped>
.AppButtonLink {
  text-decoration: none;
}

.appsContainer {
  overflow-y: scroll;
  display: flex;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
  padding: 2vh;
}
</style>
