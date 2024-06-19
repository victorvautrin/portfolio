<template>
  <div class="container">
    <slot></slot>
  </div>
</template>

<style scoped>
.container {
  background-color: rgba(0, 0, 0, 0.5);
  padding: 5px;
  padding-inline: 15px;
  border-bottom-right-radius: 20px;
  border-top-left-radius: 20px;
}
</style>
