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
        <img src="../assets/joel-show.png" alt="" srcset="">
    </div>
    <div class="items">
        <div>
            <h2>Joel Miller</h2>
        </div>
        <nav class="menu">
            <ul>
                <li>Games</li>
                <li>Feed</li>
                <li>Seguidores</li>
                <li>Seguindo</li>
            </ul>
        </nav>
        <div class="borda"></div>
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
        margin: -60px auto;
        gap: 20px;
        color: #fff;
        
    }

    .items {
        display: flex;
        flex-direction: column;
        align-items: start;
    }

    .items h2 {
        font-weight: 500;
        font-family: 'Inter', sans-serif;
        font-size: 24px;
        line-height: 29px;
    }

    .borda {
        height: 1px;
        width: 900px;
        background: #D9D9D9;
        margin-top: 10px;
    }
    .menu ul {
        display: flex;
        height: 40px;
        align-items: center;
        gap: 20px;
        color: black;
    }

    .menu ul li {
        font-family: 'Inter', sans-serif;
        font-weight: 400;
        font-size: 20px;
        line-height: 24px;
    }
</style>
