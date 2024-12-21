<template>
  <nav class="container">
    <div class="col-2">
      <div class="navbar__left">
        <i class="navbar__icon ri-menu-line"></i>
        <img class="navbar__logo" src="@/assets/image/logo.png" alt="" />
        <h1 class="navbar__title">食物銀行</h1>
      </div>
    </div>
    <div class="col-2">
      <div class="navbar__right">
        <p>台北最強美食→</p>
        <i class="ri-moon-line"></i>
        <img src="@/assets/image/user.jpg" alt="" />
      </div>
    </div>
  </nav>
</template>
<style lang="scss" scoped>
@use '@/assets/scss/_mixin.scss' as *;
@use '@/assets/scss/_var.scss' as *;
nav {
  position: fixed;
  top: 0;
  @include flex(space-between, center);
  height: 44px;
  width: 100%;
  background-color: #fff;
  border-bottom: 2px solid #eee;
}
.navbar {
  &__left {
    @include flex(left, center);
  }
  &__icon {
    font-size: 20px;
  }
  &__logo {
    object-fit: cover;
    height: 44px;
  }
  &__title {
    white-space: nowrap;
  }
  &__right {
    @include flex(right, center);
    gap: 8px;
    p {
      white-space: nowrap;
      color: rgb(184, 0, 0);
    }
    img {
      object-fit: cover;
      border-radius: 100%;
      height: 24px;
    }
  }
}
</style>
