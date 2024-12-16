<script setup>
</script>
<template>
  <header>
    <nav>
      <ul>
        <li>餐廳</li>
        <li>中式</li>
        <li>日式</li>
        <li>韓式</li>
        <li>美式</li>
        <li>其他餐飲</li>
      </ul>
      <div class="logo-item">
        <img src="../assets/image/logo.png" alt="">
        <h1>食物銀行</h1>
      </div>
      <div class="icon-item">
        <p>50元也能吃</p>
        <i class="ri-eye-line"></i>
        <i class="ri-kakao-talk-line"></i>
        <i class="ri-briefcase-3-line"></i>
        <div>
          <p>你的名字</p>
          <i class="ri-arrow-down-s-line"></i>
        </div>
      </div>
    </nav>
  </header>
</template>
<style lang="scss">
  nav{
    display: flex;
    align-items: center;
    background: white;
    padding: 0 16px;
  }
  ul{
      display: flex;
      column-gap: 4px;
      flex: 1;
    }
  h1{
    color: #9C9696;
    font-size: 20px;
  }
  .icon-item{
    display: flex;
    align-items: center;
    justify-content: right;
    column-gap: 24px;
    flex: 1;
  }
  .logo-item{
      display: flex;
      align-items: center;
      justify-content: center;
      flex: 1;
      img{
        height: 60px;
      }
  }
</style>