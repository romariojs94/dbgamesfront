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
<section class="perfil">
    <div class="profile">
        <img src="" alt="" srcset="">
        <p>Joel Miller</p>
    </div>
    <ul>
        <li>Games</li>
        <li>Feed</li>
        <li>Seguidores</li>
        <li>Seguindo</li>
    </ul>
</section>

</template>

<style>
    .banner {
        height: 350px;
        width: 100%;
        background-image: url("../assets/bg-banner.png");
    }
</style>
