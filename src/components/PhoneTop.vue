<script setup></script>

<template>
  <div class="phoneTopInfo">
    <div>
      <span class="phoneTop_item" id="phoneTopInfo_time">10:10</span>
    </div>
    <div>
      <span class="phoneTop_item" id="phoneTopInfo_connection">4G</span>
      <span class="phoneTop_item" id="phoneTopInfo_battery">100% 🔋</span>
    </div>
  </div>
</template>

<style scoped>
.phoneTop_item {
  margin-inline: 1vh;
}
.phoneTopInfo {
  display: flex;
  width: 100%;
  justify-content: space-between;
  background-color: rgba(0, 0, 0, 1);
  box-shadow: 0px 2px 1px 0px rgba(0, 0, 0, 0.5);
  color: white;
  font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
}
</style>
