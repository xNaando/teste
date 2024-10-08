<template>
  <div class="container">
    <div class="header">Bem-vindo ao Pet-Shop!</div>
    <div class="highlighted-products">
      <h2>Produtos em Destaque</h2>
      <ul>
        <li>Camas para cães</li>
        <li>Roupas para gatos</li>
        <li>Brinquedos interativos</li>
        <li>Ração premium</li>
      </ul>
    </div>
  </div>
</template>
<script setup lang="ts">
</script>
<style scoped>
.container {
  max-width: 800px;
  margin: 0 auto;
  padding: 20px;
  font-family: Arial, sans-serif;
  background-color: #f9f9f9;
  border-radius: 8px;
  box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
}

.header {
  font-size: 2.5em;
  text-align: center;
  color: #4CAF50;
  margin-bottom: 20px;
}

.highlighted-products {
  margin-bottom: 30px;
}

.highlighted-products h2 {
  color: #333;
}

.highlighted-products ul {
  list-style-type: none;
  padding: 0;
}

.highlighted-products li {
  background: #e0f7fa;
  margin: 5px 0;
  padding: 10px;
  border-radius: 5px;
}
</style>


