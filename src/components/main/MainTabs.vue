<template>
  <div>
    <ul class="list">
      <li class="list__title">台灣美食</li>
      <li class="list__title">日本美食</li>
      <li class="list__title">韓國美食</li>
      <li class="list__title">英國美食</li>
    </ul>
    <div class="container">
      <div class="container__inner">
        <div class="list__img">
          <img class="" src="@/assets/image/taiwan.jpg" alt="" />
        </div>
        <ul class="list__img__list">
          <li class="list__img__list__title">台北最強美食→</li>
          <li class="list__img__list__title">台南古都建城400年古早味美食這裡看→</li>
          <li class="list__img__list__title">台北最強美食→</li>
        </ul>
      </div>
    </div>
    <div class="list">
      <div class="list__inner">
        <div class="list__group">
          <div class="list__icon">
            <img src="@/assets/image/icon/position-icon.png" alt="" />
          </div>
          <div>
            <h2 class="list__icon__title">地區找美食</h2>
            <span class="list__icon__content">找周圍附近</span>
          </div>
        </div>
        <div class="list__group">
          <div class="list__icon">
            <img src="@/assets/image/icon/search-icon.png" alt="" />
          </div>
          <div>
            <h2 class="list__icon__title">詢問專區</h2>
            <span class="list__icon__content">找到好解答</span>
          </div>
        </div>
        <div class="list__group">
          <div class="list__icon">
            <img src="@/assets/image/icon/cake-icon.png" alt="" />
          </div>
          <div>
            <h2 class="list__icon__title">找甜點</h2>
            <span class="list__icon__content">甜蜜你的味蕾</span>
          </div>
        </div>
        <div class="list__group">
          <div class="list__icon">
            <img src="@/assets/image/icon/tea-icon.png" alt="" />
          </div>
          <div>
            <h2 class="list__icon__title">喝好茶</h2>
            <span class="list__icon__content">回甘茶在這裡</span>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<style lang="scss" scoped>
@use 'sass:color';
@use '@/assets/scss/_mixin.scss' as *;
@use '@/assets/scss/_var.scss' as *;
@use '@/assets/scss/_base.scss' as *;
.container {
  &__inner {
    border-bottom: 1px solid color.adjust($second-color, $lightness: 30%);
  }
}
.list {
  @include flex(left, center);
  &__title {
    width: 25%;
    text-align: center;
    line-height: 20px;
    padding: 12px 12px;
    background-color: color.adjust($theme-color, $lightness: 30%);
  }
  &__img {
    padding: 16px 0px;
    img {
      object-fit: cover;
      width: 100%;
      border-radius: 8px;
    }
  }
  &__img__list {
    &__title {
      @include flex(left, center);
      margin-bottom: 12px;
      font-size: 14px;
      &::before {
        content: '';
        display: inline-block;
        position: relative;
        top: -3px;
        width: 6px;
        height: 6px;
        margin-right: 4px;
        border: 2px solid #ff7800;
        border-radius: 50%;
      }
    }
  }
}
.list__inner {
  display: flex;
  padding: 0 16px;
  gap: 40px;
  overflow: auto;
}
.list__group {
  display: flex;
  align-items: center;
  gap: 8px;
}
.list__icon {
  margin-top: 16px;
  margin-bottom: 8px;
  padding: 4px 6px;
  border-radius: 100%;
  border: 1px solid color.adjust($second-color, $lightness: 30%);
  img {
    width: 32px;
  }
  &__title {
    font-size: 14px;
    line-height: 20px;
    font-weight: 700;
    white-space: nowrap;
  }
  &__content {
    font-size: 12px;
    line-height: 18px;
    white-space: nowrap;
  }
}
</style>
