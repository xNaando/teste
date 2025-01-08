<template>
  <q-layout v-if="$q.screen.width < 600" view="hHh lpR fFf">
    <q-header elevated class="bg-white text-white">
      <q-toolbar>
        <div class="row justify-center items-center col-12">
          <div>
            <q-img :src="logo" alt="img" style="height: 50px; width: 70px"/>
          </div>
          <div class="text-blue-4 q-ml-md" style="font-size: 25px">
            Serviços Náuticos
          </div>
        </div>
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
</template>

<script setup>
import logo from '/public/images/logo.png'

</script>

<style scoped>
.q-header {
  padding: 10px 20px;
}
</style>
