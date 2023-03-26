<script setup>
  import { ref } from 'vue'

  defineProps({
    msg: String,
  })

const count = ref(0)
</script>

<template>
  <div class="button">
    <p>Lista de jogos</p>
    <button>
      <img src="../assets/PlusSquareFill.svg" alt="">
      Adicionar novos jogos
    </button>
  </div>
</template>

<style>
 .button {
  margin-top: 60px;
  margin-bottom: 4px;
  max-width: 1200px;
  margin-left: auto;
  margin-right: auto;
 }
 .button p {
  font-family: "Inter", sans-serif;
  font-weight: 500;
  font-size: 14px;
  text-align: left;
  margin-bottom: 4px;
 }

 button {
  display: flex;
  border-radius: 4px;
  gap: 8px;
  width: 300px;
  height: 60px;
  justify-content: center;
  align-items: center;
  background: #0070D1;
  font-family: "Inter", sans-serif;
  font-weight: 500;
  font-size: 16px;
  color: #FFF;
  border: none;
  cursor: pointer;
 }

</style>