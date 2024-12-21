<script setup>
import search from './MainSearch.vue'
import tabs from './MainTabs.vue'
</script>

<template>
  <main>
    <search />
    <tabs />
  </main>
</template>
<style lang="scss" scoped>
@use '@/assets/scss/_var.scss' as *;
@use '@/assets/scss/_col.scss' as *;
// div {
//   background: $theme-color;
//   height: 300px;
//   width: 100%;
// }
.row {
  display: flex;
}
</style>
