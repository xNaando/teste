<template>
  <div class="container">
    <div class="oi">
      <img class="foto" :src="img4" alt="img" />
      <img class="foto" :src="img1" alt="img" />
      <img class="foto" :src="img2" alt="img" />
      <img class="foto" :src="img3" alt="img" />
    </div>
  </div>
</template>

<script setup lang="ts">
import img1 from '/public/1.png';
import img2 from '/public/2.png';
import img3 from '/public/3.png';
import img4 from '/public/4.png';
</script>

<style scoped>
.container {
  display: flex; /* Ativa o layout flex */
  justify-content: center; /* Centraliza horizontalmente */
  align-items: center; /* Centraliza verticalmente */
  width: 100%; /* Ocupa toda a largura da tela */
}

.oi {
  display: flex; /* Ativa o layout flex */
  flex-direction: column; /* Organiza os itens em coluna */
  align-items: center; /* Centraliza os itens na coluna */
  width: 500px; /* Define uma largura fixa */
}

.foto {
  max-width: 100%;
  object-fit: contain;
}
</style>
