<script setup>
import { ref } from 'vue'

defineProps({
  msg: String,
})

const count = ref(0)
</script>

<template> 
  <header class="banner">
      
  </header>
  <section class="profile">
    <div class="profile-img">
      <img src="../assets/joel-show.png" alt="">
    </div>
    <div class="profile-items">
      <h2>Joel Miller</h2>
      <nav class="menu">
        <ul>
          <li>Games</li>
          <li>Feed</li>
          <li>Seguidores</li>
          <li>Seguindo</li>
        </ul>
      </nav>
    </div>
  </section>   
  
</template>
<style>
  .banner {
      height: 350px;
      width: auto;
      background: url("../assets/bg-banner.jpg") no-repeat center center;
      background-size: cover;
  }
  .profile {
      display: flex;
      max-width: 1200px;
      margin-top: -60px;
      margin-right: auto;
      margin-left: auto;
      gap: 20px;
      color: #fff;
  }
  .profile-items {
    display: flex;
    flex-direction: column;
    height: 99px;
    justify-content: space-between;
  }
  .profile-items h2 {
      margin-top: 18px;
      font-weight: 500;
      font-family: 'Inter', sans-serif;
      font-size: 24px;
      color: #FFF;
  }  
  .borda {
      height: 1px;
      width: 900px;
      background: #D9D9D9;
      margin-top: 10px;
  }
  .menu {
    border-bottom: 1px solid rgba(217, 217, 217, 0.8);
    width: calc(1200px - 10vw);
  }
  .menu ul {
      display: flex;
      gap: 20px;
      color: #242424;
      margin-bottom: 4px;
  }
  .menu ul li {
      font-family: 'Inter', sans-serif;
      font-weight: 400;
      font-size: 18px;
      line-height: 24px;
  }
</style>
