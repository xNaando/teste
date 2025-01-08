<template>
  <div class="pagina">
    <q-layout view="hHh lpR fFf">
      <q-header v-if="$q.screen.width > 600" elevated class="bg-blue-4 text-white">
        <q-toolbar>
          <q-toolbar-title>
            Serviços Náuticos
          </q-toolbar-title>
          <div class="q-gutter-md" style="margin-left:auto;">
            <q-btn flat label="HOME" @click="navigateTo('home')"/>
            <q-btn flat label="SOBRE NÓS" @click="navigateTo('sobre-nos')"/>
            <q-btn flat label="SERVIÇOS" @click="navigateTo('servicos')"/>
            <q-btn flat label="PINTURAS NÁUTICAS" @click="navigateTo('pinturas-nauticas')"/>
            <q-btn flat label="CONTATO" @click="navigateTo('contato')"/>
          </div>
        </q-toolbar>
      </q-header>
      <q-header v-if="$q.screen.width < 600" elevated class="bg-blue-4 text-white">
        <q-toolbar>
          <q-toolbar-title class="text-center">
            Serviços Náuticos
          </q-toolbar-title>
        </q-toolbar>
      </q-header>
      <div class="col-12" style="margin-top: 70px">
        <div id="home" style="height: 100vh; background: lightblue;">
          Home Section
        </div>
        <div id="contato" style="height: 100vh; background: lightgreen;">
          Contato Section
        </div>
        <div id="pinturas-nauticas" style="height: 100vh; background: lightcoral;">
          Pinturas Náuticas Section
        </div>
        <div id="servicos" style="height: 100vh; background: lightgoldenrodyellow;">
          Serviços Section
        </div>
        <div id="sobre-nos" style="height: 100vh; background: lightpink;">
          Sobre Nós Section
        </div>
        <div id="nossos-barcos" style="height: 100vh; background: lightseagreen;">
          Nossos Barcos Section
        </div>
      </div>
    </q-layout>
  </div>
</template>

<script setup>
import {ref} from 'vue'

const drawerOpen = ref(false)

const navigateTo = (section) => {
  if (section === 'home') {
    window.scrollTo({top: 0, behavior: 'smooth'})
  } else {
    const element = document.getElementById(section)
    if (element) {
      element.scrollIntoView({behavior: 'smooth'})
    }
  }
}
</script>

<style scoped>
.q-header {
  padding: 10px 20px;
}

.q-btn {
  font-size: 16px;
  font-weight: 500;
}

.pagina {
  overflow: hidden;
}
</style>
