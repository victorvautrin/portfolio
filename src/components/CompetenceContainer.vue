<script setup>
import { ref } from 'vue'
const props = defineProps(['level', 'nom'])

const levelNames = {
  1: 'Débutant',
  2: 'Intermédiaire',
  3: 'Avancé'
}

const levelText = ref(levelNames[Number(props.level)])
const competenceName = ref(props.nom)
</script>

<template>
  <div class="competenceContainer">
    <span class="competenceTitre">{{ competenceName }}</span>
    <span :class="['competenceNiveau', 'level' + props.level]">{{ levelText }}</span>
  </div>
</template>

<style scoped>
.competenceContainer {
  background-color: rgba(0, 0, 0, 0.5);
  padding: 5%;
  border-bottom-right-radius: 10px;
  border-top-left-radius: 10px;
  color: white;
  text-align: end;
  display: flex;
  justify-content: space-between;
}

.level1 {
  color: #ff3030;
}

.level2 {
  color: #fff944;
}

.level3 {
  color: #48ff48;
}
</style>
