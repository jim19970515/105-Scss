<template>
  <div class="container">
    <div class="search-input">
      <span>關鍵字 (例：食物名稱、餐廳名、地區...)</span>
      <i class="ri-search-line"></i>
    </div>
  </div>
</template>
<style lang="scss" scoped>
@use '@/assets/scss/_mixin.scss' as *;
@use '@/assets/scss/_var.scss' as *;
.container {
  background-color: $lightened-theme-color;
  padding: 16px;
}
.search-input {
  @include flex(space-between, center);
  background-color: #fff;
  border: 1px solid $theme-color;
  cursor: pointer;
  border-radius: 0.25rem;
  padding: 8px 12px;
  white-space: nowrap;
  span {
    text-align: left;
    overflow: hidden;
    color: $second-color;
    font-size: 16px;
    font-weight: 700;
  }
  i {
    text-align: right;
    font-size: 28px;
  }
}
</style>
