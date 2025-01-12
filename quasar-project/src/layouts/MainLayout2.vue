<template>
  <div class="container">
    <div class="oi">
      <img class="foto" :src="img1" alt="img" />
      <img class="foto" :src="img2" alt="img" />
      <img class="foto" :src="img3" alt="img" />
      <img class="foto" :src="img4" alt="img" />
      <img class="foto" :src="img5" alt="img" />
      <img class="foto" :src="img6" alt="img" />
      <img class="foto" :src="img7" alt="img" />
    </div>
  </div>
</template>

<script setup lang="ts">
import img1 from '/public/1.gif';
import img2 from '/public/2.gif';
import img3 from '/public/3.gif';
import img4 from '/public/4.gif';
import img5 from '/public/5.gif';
import img6 from '/public/6.png';
import img7 from '/public/7.gif';
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
