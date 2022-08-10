<script setup lang="ts">

</script>

<template>
  <h3 id="grid">
    Grid Layout
  </h3>
  <div class="ctn">
    <div class="header">
      header
    </div>
    <div class="nav">
      nav
    </div>
    <div class="body">
      body
    </div>
    <div class="footer">
      footer
    </div>
  </div>
</template>

<style scoped>
#grid {
  margin: 0.75rem 0;
  color: blue;
}
.ctn {
  display: grid;
  border: 1px gray solid;
  width: 22.5rem;
  height: 22.5rem;
  grid-gap: 10px;
  grid-template-rows: repeat(5, 1fr);
  grid-template-columns: repeat(5, 1fr);
}
.header {
  grid-row-start: 1;
  grid-row-end: 1;
  grid-column-start: 1;
  grid-column-end: 6;
  background: blue;
}
.nav {
  grid-row-start: 2;
  grid-row-end: 5;
  grid-column-start: 1;
  grid-column-end: 2;
  background: green;
}
.body {
  grid-row-start: 2;
  grid-row-end: 5;
  grid-column-start: 2;
  grid-column-end: 6;
  background: yellow;
}
.footer {
  grid-row-start: 5;
  grid-row-end: 5;
  grid-column-start: 1;
  grid-column-end: 6;
  background: pink;
}
</style>
