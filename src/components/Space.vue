<script setup lang="ts">

</script>

<template>
  <div id="space">
    <p>
      Space
    </p>
    <div class="bg-img" alt="" />
  </div>
</template>

<style scoped>
#space {
  margin: 0.75rem 0;
}
p {
  padding: 12px;
  width: calc(50% - 32px);
  border: 3px purple dashed;
  border-radius: 12px;
}
.bg-img {
  margin: 0.75rem 0;
  aspect-ratio: 5 / 3;
  background-image: url('https://source.unsplash.com/collection/94734566/1920x1080');
}
</style>
