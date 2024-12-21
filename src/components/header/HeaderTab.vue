<script setup>
import { reactive } from 'vue'
const tabArray = reactive(['台式', '日式', '韓式', '美式', '英式', '印度'])
</script>

<template>
  <div class="container">
    <div class="list">
      <ul>
        <li v-for="(item, i) in tabArray" :key="i" :class="item == '台式' ? 'focus' : ''">
          {{ item }}
        </li>
      </ul>
    </div>
  </div>
</template>
<style lang="scss" scoped>
@use '@/assets/scss/_mixin.scss' as *;
@use '@/assets/scss/_var.scss' as *;
.container {
  margin-top: 46px;
}
.list {
  padding: 15px 0;
  ul {
    @include flex(space-between, center);
    gap: 16px;
  }
  li {
    color: $second-dark-color;
    font-weight: 800;
    cursor: pointer;
    &.focus {
      color: $theme-color !important;
    }
  }
}
</style>
