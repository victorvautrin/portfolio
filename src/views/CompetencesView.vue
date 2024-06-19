<script setup>
import GenericContainer from '@/components/GenericContainer.vue'
import CompetenceContainer from '@/components/CompetenceContainer.vue'
</script>

<template>
  <div class="competencesView">
    <div id="competencesView_content">
      <GenericContainer>
        <h3>Langages & Frameworks</h3>
      </GenericContainer>
      <ul class="competenceList">
        <li class="competenceListItem"><CompetenceContainer nom="Python" :level="3" /></li>
        <li class="competenceListItem"><CompetenceContainer nom="Lua" :level="3" /></li>
        <li class="competenceListItem"><CompetenceContainer nom="VueJS" :level="3" /></li>

        <li class="competenceListItem"><CompetenceContainer nom="HTML/CSS" :level="2" /></li>
        <li class="competenceListItem"><CompetenceContainer nom="SQL" :level="2" /></li>
        <li class="competenceListItem"><CompetenceContainer nom="PHP" :level="2" /></li>
        <li class="competenceListItem"><CompetenceContainer nom="JavaScript" :level="2" /></li>
        <li class="competenceListItem"><CompetenceContainer nom="Java" :level="2" /></li>

        <li class="competenceListItem"><CompetenceContainer nom="Kotlin" :level="1" /></li>
        <li class="competenceListItem"><CompetenceContainer nom="C" :level="1" /></li>
      </ul>

      <GenericContainer>
        <h3>Logiciels</h3>
      </GenericContainer>
      <ul class="competenceList">
        <li class="competenceListItem"><CompetenceContainer nom="Suite Office" :level="3" /></li>
        <li class="competenceListItem">
          <CompetenceContainer nom="Visual Studio Code" :level="3" />
        </li>

        <li class="competenceListItem"><CompetenceContainer nom="PowerAMC" :level="2" /></li>
        <li class="competenceListItem"><CompetenceContainer nom="NetBeans" :level="2" /></li>
        <li class="competenceListItem"><CompetenceContainer nom="SQL Developper" :level="2" /></li>
        <li class="competenceListItem"><CompetenceContainer nom="VMWare" :level="2" /></li>

        <li class="competenceListItem"><CompetenceContainer nom="Code::Blocks" :level="1" /></li>
        <li class="competenceListItem"><CompetenceContainer nom="PhpStorm" :level="1" /></li>
      </ul>
    </div>
  </div>
</template>

<style scoped>
.competencesView {
  overflow-y: scroll;
  width: 100%;
  height: 100%;
  background-color: rgb(85, 45, 45);
  z-index: -20;
  color: white;
}

.competenceListItem {
  margin-block: 5%;
}

ul {
  list-style-type: none;
}

#competencesView_content {
  margin: 10px;
  text-align: justify;
}
</style>
