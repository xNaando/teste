<template>
  <q-layout v-if="$q.screen.width > 600" view="hHh lpR fFf">
    <q-header elevated class="bg-white text-white">
      <q-toolbar>
        <div class="row items-center col-12">
          <div class="row col-4 items-center">
            <div>
              <q-img :src="logo" alt="img" style="height: 50px; width: 70px"/>
            </div>
            <div class="text-blue-4 q-ml-md" style="font-size: 25px">
              Serviços Náuticos
            </div>
          </div>
          <div class="row col-8 justify-end text-blue-4">
            <q-btn flat label="HOME" @click="navigateTo('home')"/>
            <q-btn flat label="SOBRE NÓS" @click="navigateTo('sobre-nos')"/>
            <q-btn flat label="SERVIÇOS" @click="navigateTo('servicos')"/>
            <q-btn flat label="PINTURAS NÁUTICAS" @click="navigateTo('pinturas-nauticas')"/>
            <q-btn flat label="CONTATO" @click="navigateTo('contato')"/>
            <q-btn flat label="LOCALIZAÇÃO" @click="navigateTo('localizacao')"/>
          </div>
        </div>
      </q-toolbar>
    </q-header>
    <div class="row col-12" style="margin-top: 70px">
      <div class="col-12" id="home" style="margin-top: -200px">
        <video
          class="no-margin no-padding"
          :src="video"
          autoplay
          loop
          muted
          playsinline
          style="height: 100%; width: 100%;"
        ></video>
      </div>
      <div class="row col-12" id="sobre-nos" style="margin-top: 100px">
        <div class="col-6">
          <q-img :src="sobrenos" alt="img" style="height: 497px; width: 648px"/>
        </div>
        <div class="row col-6">
          <div class="col-12 text-blue-4" style="font-size: 46px; font-weight: bold;">
               SOBRE NÓS
          </div>
          <div class="row col-12" style="font-size: 13px">
            <div class="col-12">
              A Nova Onda Pinturas foi fundada em 1962 por José Domingos Simões. Em 1990, seu filho Joacir José Simões,
              assumiu o comando da empresa dando continuidade até os dias de hoje.
            </div>
            <div class="col-12">
              Com o passar dos anos, a paixão por embarcações ficou cada vez maior. Em 2008 passamos a produzir
              embarcações de esporte e recreio sob encomenda, sempre prezando pela qualidade e segurança.
            </div>
            <div class="col-12">
              Nossa equipe é altamente treinada e capacitada para atuar nas áreas de laminação, pintura, marcenaria,
              polimento, projeto, modelação e engenharia. Lidamos com qualquer parte da embarcação garantindo um trabalho
              da mais alta qualidade. Estamos localizados no Joinville Iate Clube e possuímos uma ampla infraestrutura.
            </div>
            <div class="col-12">
              Possuímos carreta que suporta veleiro e embarcações de pequeno e grande porte. Além de nosso espaço,
              contamos com uma equipe móvel e executamos trabalhos na sua própria marina ou estaleiro.
            </div>
            <div class="col-12">
              Se pensa em comprar ou reformar a sua embarcação, nós podemos te atender! Conheça nossos produtos e
              surpreenda-se com a qualidade e o acabamento. São barcos versáteis e seguros que podem ser facilmente
              adequados ao gosto do cliente.
            </div>
          </div>
          <div class="col-12 text-blue-4" style="font-size: 18px; margin-top: 30px">
            FAZER DOS SEUS MOMENTOS DE ESPORTE E LAZER NÁUTICO UMA EXPERIÊNCIA AGRADÁVEL É NOSSA OBRIGAÇÃO!
          </div>
        </div>
      </div>
      <div class="col-12" id="servicos">
        Serviços
      </div>
      <div class="col-12" id="pinturas-nauticas">
        Pinturas Náuticas
      </div>
      <div class="col-12" id="servicos">
        Contato
      </div>
      <div class="col-12" id="localizacao">
        Localizacao
      </div>
    </div>
  </q-layout>
</template>

<script setup>
import logo from '/public/images/logo.png'
import sobrenos from '/public/images/sobrenos.png'
import video from '/public/images/video.mp4'

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
</style>
