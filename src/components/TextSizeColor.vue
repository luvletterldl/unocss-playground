<script setup lang="ts">

</script>

<template>
  <div id="text-size-color">
    <h3>
      Text Size Color
    </h3>
    <p class="sm">
      sm text
    </p>
    <p class="lg">
      lg text
    </p>
    <p class="xl">
      xl text
    </p>
    <p class="txl">
      3xl text
    </p>
    <p text-16px>
      16px text
    </p>
    <p class="slg">
      9xl text
    </p>
  </div>
  <div class="text">
    Lorem ipsum dolor sit amet, consectetur adipiscing elit.Lorem ipsum dolor sit amet, consectetur adipiscing elit.Lorem ipsum dolor sit amet, consectetur adipiscing elit.Lorem ipsum dolor sit amet, consectetur adipiscing elit.
  </div>
</template>

<style scoped>
#text-size-color {
  text-align: right;
}
p {
  display: inline-block;
  margin: 0 0.75rem;
  padding: 0.75rem;
}
.sm {
  font-size: 0.875rem;
  line-height: 1.25rem;
}
.sm:hover {
  transform: scale(2);
}
.lg {
  font-size: 1.25rem;
  line-height: 1.5rem;
}
.xl {
  font-size: 1.5rem;
  line-height: 1.75rem;
  color: rgba(0,0,0 ,0.3);
}
.xl:hover {
  color: rgba(0,0,0 ,0.5);
}

.txl {
  font-size: 2rem;
  line-height: 2.5rem;
  text-shadow: 1.2rem;
}

.slg {
  font-size: 9rem;
  line-height: 9rem;
  background: linear-gradient(to right, violet, fuchsia);
}
.slg:hover {
  background: linear-gradient(to right, purple, pink);
}

.text {
  width: 33%;
  display: -webkit-box;
  -webkit-box-orient: vertical;
  text-overflow: ellipsis;
  overflow: hidden;
  -webkit-line-clamp: 2;
}
</style>
