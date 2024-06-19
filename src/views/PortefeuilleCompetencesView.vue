<script setup>
import GenericContainer from '@/components/GenericContainer.vue'
</script>

<template>
  <div class="competencesView">
    <div id="competencesView_content">
      <GenericContainer>
        <h3>Portefeuille de Compétences</h3>
      </GenericContainer>
      <br />
      <!--============================================-->
      <ul>
        <GenericContainer>
          <h3>Réaliser</h3>
        </GenericContainer>
        <ul>
          <li>
            <GenericContainer> Développer des applications informatiques simples </GenericContainer>
          </li>
          <li>
            <GenericContainer>
              Partir des exigences et aller jusqu'à une application complète
            </GenericContainer>
          </li>
        </ul>
      </ul>
      <!--============================================-->
      <ul>
        <GenericContainer>
          <h3>Optimiser</h3>
        </GenericContainer>
        <ul>
          <li>
            <GenericContainer> Appréhender et construire des algorithmes </GenericContainer>
          </li>
          <li>
            <GenericContainer>
              Sélectionner les algorithmes adéquats pour répondre à un problème donné
            </GenericContainer>
          </li>
        </ul>
      </ul>
      <!--============================================-->
      <ul>
        <GenericContainer>
          <h3>Administrer</h3>
        </GenericContainer>
        <ul>
          <li>
            <GenericContainer> Installer et configurer un poste de travail </GenericContainer>
          </li>
          <li>
            <GenericContainer>
              Déployer les services dans une architecture réseau
            </GenericContainer>
          </li>
        </ul>
      </ul>
      <!--============================================-->
      <ul>
        <GenericContainer>
          <h3>Gérer</h3>
        </GenericContainer>
        <ul>
          <li>
            <GenericContainer>
              Concevoir et mettre en place une base de données à partir d'un cahier des charges
              client
            </GenericContainer>
          </li>
          <li>
            <GenericContainer>
              Optimiser une base de données, interagir avec une application et mettre en oeuvre la
              sécurité
            </GenericContainer>
          </li>
        </ul>
      </ul>
      <!--============================================-->
      <ul>
        <GenericContainer>
          <h3>Conduire</h3>
        </GenericContainer>
        <ul>
          <li>
            <GenericContainer>
              Identifier les besoins métiers des clients et des utilisateurs
            </GenericContainer>
          </li>
          <li>
            <GenericContainer>
              Appliquer une démarche de suivi de projet en fonction des besoins métiers des clients
              et des utilisateurs
            </GenericContainer>
          </li>
        </ul>
      </ul>
      <!--============================================-->
      <ul>
        <GenericContainer>
          <h3>Collaborer</h3>
        </GenericContainer>
        <ul>
          <li>
            <GenericContainer>
              Identifier ses aptitudes pour travailler dans une équipe
            </GenericContainer>
          </li>
          <li>
            <GenericContainer>
              Situer son rôle et ses missions au sein d'une équipe informatique
            </GenericContainer>
          </li>
        </ul>
      </ul>
      <!--============================================-->
    </div>
  </div>
</template>

<style scoped>
.competencesView {
  overflow-y: scroll;
  width: 100%;
  height: 100%;
  background-color: rgb(63, 100, 130);
  z-index: -20;
  color: white;
}

.competenceListItem {
  margin-block: 5%;
}

ul {
  list-style-type: none;
  margin-block: 2px;
  color: rgb(39, 255, 39);
}

li {
  margin-block: 5px;
  color: white;
}

#competencesView_content {
  margin: 10px;
  text-align: justify;
}
</style>
