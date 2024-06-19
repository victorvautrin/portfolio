<script setup>
const props = defineProps(['resultat', 'nom'])
</script>

<template>
  <div class="competenceContainer">
    <span class="competenceTitre">{{ props.nom }}</span>
    <span class="competenceNiveauMini">{{ props.resultat }}</span>
  </div>
</template>

<style scoped>
.competenceContainer {
  background-color: rgba(0, 0, 0, 0.5);
  padding: 5%;
  border-bottom-right-radius: 10px;
  border-top-left-radius: 10px;
  color: white;
  text-align: start;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}

.competenceNiveauMini {
  color: rgb(13, 255, 0);
}
</style>
