<script setup>
import navber from './HomeNavber.vue';
</script>
<template>
  <header>
    <navber/>
    <div>
      <ul class="header-tab">
        <li style="color: #E96117;">找美食</li>
        <li>早餐</li>
        <li>午餐</li>
        <li>晚餐</li>
        <li>宵夜</li>
        <li>飯後甜點</li>
      </ul>
    </div>
  </header>
</template>
<style lang="scss">
  .header-tab{
    display: flex;
    justify-content: center;
    align-items: center;
    column-gap: 40px;
    height: 70px;
    li{
      font-weight:700;
      color: #9C9696;
    }
  }
</style>