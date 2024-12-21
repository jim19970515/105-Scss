<template>
  <div class="card">
    <div class="card__body">
      <div class="card__header">
        <h1 class="card__title">蒙奇Ｄ魯夫</h1>
        <span class="card__span">前往預訂系統></span>
      </div>
      <div class="card__main">
        <div class="card__choose">
          <p>儲存的餐廳</p>
          <p>訂位紀錄</p>
        </div>
        <div class="content">
          <div class="content__inner">
            <h2 class="content__title">鼎鼎豐</h2>
            <p class="content__p">可口的小籠包專賣店</p>
          </div>
          <div class="content__inner">
            <h2 class="content__title">金拱門</h2>
            <p class="content__p">薯條界的專家</p>
          </div>
          <div class="content__inner">
            <h2 class="content__title">啃他雞</h2>
            <p class="content__p">風靡全球的葡式蛋塔店</p>
          </div>
          <p class="footer__text">更多></p>
        </div>
      </div>
    </div>
  </div>
</template>
<style lang="scss" scoped>
@use 'sass:color';
@use '@/assets/scss/_mixin.scss' as *;
@use '@/assets/scss/_var.scss' as *;
.card {
  padding: 16px;
  background-color: $lightened-theme-color;
  &__body {
    background-color: #fff;
    padding: 16px;
    border-radius: 20px;
  }
  &__header {
    @include flex(space-between, center);
    margin-bottom: 16px;
  }
  &__title {
    font-size: 18px;
    line-height: 24px;
    font-weight: 700;
  }
  &__span {
    font-size: 16px;
    color: #1654b9;
    font-weight: 700;
  }
}
.card__choose {
  @include flex(left, center);
  border: 1px solid color.adjust($second-color, $lightness: 20%);
  border-radius: 8px;
  margin-bottom: 4px;
  p {
    width: 50%;
    line-height: 20px;
    text-align: center;
    padding: 8px 12px;
    background-color: color.adjust($theme-color, $lightness: 30%);
    font-weight: 700;
    color: $theme-color;
  }
}
.content {
  display: flex;
  flex-direction: column;
  gap: 8px;
  padding: 16px;
  &__title {
    color: #1654b9;
    font-size: 16px;
    line-height: 28px;
    font-weight: 700;
  }
  &__p {
    color: $second-color;
    font-size: 12px;
    line-height: 18px;
    font-weight: 400;
  }
}
.footer__text {
  margin-top: 8px;
  font-size: 16px;
  line-height: 28px;
  font-weight: 700;
  text-align: center;
  color: $second-color;
}
</style>
