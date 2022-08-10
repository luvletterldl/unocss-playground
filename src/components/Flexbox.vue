<script setup lang="ts">

</script>

<template>
  <div id="flexbox">
    <p class="title">
      FlexBox
    </p>
    <div class="ctn">
      <p class="left">
        left
      </p>
      <p class="center">
        center
      </p>
      <p class="right">
        right
      </p>
    </div>
  </div>
</template>

<style scoped>
.title {
  margin: 00.75rem;
  color: purple;
}

.ctn {
  display: flex;
  flex: column;
  align-items: center;
  justify-content: space-evenly;
  border-radius: 12px;
}
.left, .right {
  width: 100px;
  background: pink;
  text-align: center;
}
.center {
  text-align: center;
  width: 100%;
}
</style>
