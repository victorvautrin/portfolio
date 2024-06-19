<script setup></script>

<template>
  <div class="contactView">
    <div id="contactView_content">
      <p>Pour entrer en contact avec moi, veuillez me contacter sur cette addresse:</p>
      <form>
        <a href="mailto:vautrinvic@gmail.com">vautrinvic@gmail.com</a>
      </form>
    </div>
  </div>
</template>

<style scoped>
.contactView {
  overflow-y: hidden;
  width: 100%;
  height: 100%;
  background-color: rgb(23, 36, 69);
  z-index: -20;
  text-decoration: none;
  color: rgb(209, 209, 209);
}

#contactView_content {
  margin: 10px;
  text-align: justify;
}

a {
  text-decoration: none;
  color: rgb(255, 255, 255);
  font-weight: bolder;
  font-size: 1.5rem;
}
</style>
