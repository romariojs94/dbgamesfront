<script setup>
  import { ref } from 'vue'

  defineProps({
    msg: String,
  })

  const count = ref(0)
</script>

<template>
  <div class="games-list">
    <h3>Todos os meus Games</h3>
    <div class="games-list-grid">
      <div class="games-list-child">
        <a href="/">
          <img src="../assets/horizon.jpg" alt="">
          <p>Horizon Forbidden West™</p>
          <ul class="etiquetas">
            <li>Ação</li>
            <li>PS4</li>
          </ul>
        </a>
      </div>
      <div class="games-list-child">
        <a href="/">
          <img src="../assets/ghost.jpg" alt="">
          <p>Ghost of Tsushima™</p>
          <ul class="etiquetas">
            <li>Ação</li>
            <li>PS5</li>
          </ul>
        </a>
      </div>
      <div class="games-list-child">
        <a href="/">
          <img src="../assets/returnal.jpg" alt="">
          <p>Returnal™</p>
          <ul class="etiquetas">
            <li>Ficção</li>
            <li>PS4</li>
          </ul>
        </a>
      </div>
      <div class="games-list-child">
        <a href="/">
          <img src="../assets/demon-souls.jpg" alt="">
          <p>Demon Souls</p>
          <ul class="etiquetas">
            <li>Mistério, Terror</li>
            <li>PS4</li>
          </ul>
        </a>
      </div>
      <div class="games-list-child">
        <a href="/">
          <img src="../assets/plague.jpg" alt="">
          <p>A Plague Tale</p>
          <ul class="etiquetas">
            <li>Ação, Aventura</li>
            <li>PS4</li>
          </ul>
        </a>
      </div>
      <div class="games-list-child">
        <a href="/">
          <img src="../assets/village.jpg" alt="">
          <p>Village</p>
          <ul class="etiquetas">
            <li>Suvivor horror</li>
            <li>PS4</li>
          </ul>
        </a>
      </div>
    </div>   
  </div>
</template>


<style>
  .games-list-grid {
    display: grid;
    gap: 20px;
    grid-template-columns: 1fr 1fr 1fr 1fr 1fr;
  }
  
  .games-list {
    max-width: 1200px;
    margin-left: auto;
    margin-right: auto;
    margin-top: 40px;
    margin-bottom: 80px;
  }
  .games-list h3 {
    display: inline-flex;
    gap: 4px;
    font-weight: 500;
    font-family: "Inter", sans-serif;
    font-size: 20px;
  }
  .games-list h3::before {
    content: "";
    display: inline-block;
    background: #0070D1;
    height: 24px;
    width: 4px;
  }

  .games-list p {
    margin-top: 4px;
    color: #3D3D3D;
    font-weight: 400;
    font-family: "Inter", sans-serif;
    font-size: 14px;
  }
  .games-list .etiquetas {
    display: flex;
    gap: 4px;
    margin-top: 6px;
  }
  .games-list li {
    background: #E0E0E0;
    padding: 4px 8px;
    border-radius: 4px;
    font-weight: 400;
    font-family: "Inter", sans-serif;
    font-size: 12px;
  }
</style>