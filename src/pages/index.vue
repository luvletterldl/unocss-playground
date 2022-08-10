<script setup lang="ts">
const mode = useColorMode({
  attribute: 'theme',
  modes: {
    // custom colors
    student: 'student',
    teacher: 'teacher',
  },
})
</script>

<template>
  <main>
    <header>
      <nav>
        <a href="#text-size-color">text-size-color</a>
        <a href="#grid">grid</a>
        <a href="#flexbox">flexbox</a>
        <a href="#space">space</a>
      </nav>
      <label for="switch-theme">切换主题</label>
      <select v-model="mode">
        <option value="" selected>
          默认
        </option>
        <option value="teacher">
          教师
        </option>
        <option value="student">
          学生
        </option>
      </select>
    </header>
    <text-size-color />
    <grid />
    <flexbox />
    <space />
  </main>
</template>

<style scoped>
main {
  overscroll-behavior: smooth;
  padding: 0.75rem;
}
header {
  position: sticky;
  top: 0;
  z-index: 10;
  box-shadow: 0px 0px 8px rgba(0, 0, 0, 0.25);
  backdrop-filter: blur(10px);
  display: flex;
  align-items: center;
  border: 2px var(--main) dashed;
}
nav {
  display: flex;
  flex: row nowrap;
  align-items: center;
  justify-content: space-between;
  overflow-x: auto;
  margin: 0.75rem;
}
a {
  padding: 0.75rem;
  border-radius: 12px;
  margin-right: 0.5rem;
  border: 1px var(--main) solid;
}
select {
  outline: none;
  border: 1px var(--main) solid;
  margin: 0.75rem;
}
</style>
