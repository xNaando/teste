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
        <div class="row col-6 q-pr-lg">
          <div class="row col-12 items-center">
            <div class="text-blue-4" style="font-size: 46px; font-weight: bold;">
              SOBRE NÓS
            </div>
            <div class="col" style="padding-left: 20px">
              <div style="height: 5px; background-color: #ccc; width: 100%;"></div>
            </div>
          </div>
          <div class="row col-12" style="font-size: 14px;">
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
              polimento, projeto, modelação e engenharia. Lidamos com qualquer parte da embarcação garantindo um
              trabalho
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
          <div class="col-12 text-blue-4" style="font-size: 18px; margin-top: 30px; font-weight: bold;">
            FAZER DOS SEUS MOMENTOS DE ESPORTE E LAZER NÁUTICO UMA EXPERIÊNCIA AGRADÁVEL É NOSSA OBRIGAÇÃO!
          </div>
        </div>
      </div>
      <div class="row col-12" id="servicos" style="margin-top: 100px">
        <div class="row col-12 items-center">
          <div class="text-blue-4" style="font-size: 46px; font-weight: bold; padding-left: 30px">
            NOSSOS SERVIÇOS
          </div>
          <div class="col" style="padding-left: 20px; padding-right: 20px;">
            <div style="height: 5px; background-color: #ccc; width: 100%;"></div>
          </div>
        </div>
        <div class="row col-12 q-pl-lg q-mt-lg">
          <div class="row col-12 q-pa-lg bg-blue-4 text-white" style="font-size: 15px">
            <div class="col">
              01. Reparos em fibra de vidro
            </div>
            <div class="col">
              02. Tratamento de Osmose
            </div>
            <div class="col">
              03. Pintura e retoque em gel coats
            </div>
            <div class="col">
              04. Letreiros
            </div>
          </div>
          <div class="col-12" style="height: 5px"/>
          <div class="row col-12 q-pa-lg bg-blue-4 text-white" style="font-size: 15px">
            <div class="col">
              05. Pintura de faixas personalizadas
            </div>
            <div class="col">
              06. Alongamento de plataforma
            </div>
            <div class="col">
              07. Troca de sicaflex
            </div>
            <div class="col">
              08. Polimento com espelhamento
            </div>
          </div>
          <div class="col-12" style="height: 5px"/>
          <div class="row col-12 q-pa-lg bg-blue-4 text-white" style="font-size: 15px">
            <div class="col">
              09. Lixamento de Teka
            </div>
            <div class="col">
              10. Aplicação de tinta anti-crustante
            </div>
            <div class="col">
              11. Modificação estrutural
            </div>
            <div class="col">
              12. Aplicação de Propspeed
            </div>
          </div>
          <div class="col-12" style="height: 5px"/>
          <div class="row col-12 q-pa-lg bg-blue-4 text-white" style="font-size: 15px">
            <div class="col">
              13. Fabricação de plataforma submergível
            </div>
            <div class="col">
              14. Fabricação de teka
            </div>
            <div class="col">
              15. Fabricação espaço gourmand
            </div>
            <div class="col">
              16. Fabricação HARD TOP
            </div>
          </div>
        </div>
      </div>
      <div class="row col-12" id="pinturas-nauticas" style="margin-top: 100px">
        <div class="row col-12 items-center">
          <div class="text-blue-4" style="font-size: 46px; font-weight: bold; padding-left: 30px">
            PINTURAS NÁUTICAS
          </div>
          <div class="col" style="padding-left: 20px; padding-right: 20px;">
            <div style="height: 5px; background-color: #ccc; width: 100%;"></div>
          </div>
        </div>
        <div class="row col-12">
          <div class="col q-pa-md" style="cursor: pointer">
            <q-img @click="img1Grande = true" :src="img1" alt="img" style="height: 100%; width: 100%"/>
            <q-dialog v-model="img1Grande">
              <div style="height: auto; width: 100%; max-width: 1202px; overflow: hidden;">
                <q-img @click="img1Grande = false" :src="img1x1" alt="img"
                       style="height: auto; width: 100%; cursor: pointer"/>
              </div>
            </q-dialog>
          </div>
          <div class="col q-pa-md" style="cursor: pointer">
            <q-img @click="img2Grande = true" :src="img2" alt="img" style="height: 100%; width: 100%"/>
            <q-dialog v-model="img2Grande">
              <div style="height: auto; width: 100%; max-width: 1202px; overflow: hidden;">
                <q-img @click="img2Grande = false" :src="img1x2" alt="img"
                       style="height: auto; width: 100%; cursor: pointer"/>
              </div>
            </q-dialog>
          </div>
          <div class="col q-pa-md" style="cursor: pointer">
            <q-img @click="img3Grande = true" :src="img3" alt="img" style="height: 100%; width: 100%"/>
            <q-dialog v-model="img3Grande">
              <div style="height: auto; width: 100%; max-width: 1202px; overflow: hidden;">
                <q-img @click="img3Grande = false" :src="img1x3" alt="img"
                       style="height: auto; width: 100%; cursor: pointer"/>
              </div>
            </q-dialog>
          </div>
        </div>
        <div class="row col-12">
          <div class="col q-pa-md" style="cursor: pointer">
            <q-img @click="img4Grande = true" :src="img4" alt="img" style="height: 100%; width: 100%"/>
            <q-dialog v-model="img4Grande">
              <div style="height: auto; width: 100%; max-width: 1202px; overflow: hidden;">
                <q-img @click="img4Grande = false" :src="img1x4" alt="img"
                       style="height: auto; width: 100%; cursor: pointer"/>
              </div>
            </q-dialog>
          </div>
          <div class="col q-pa-md" style="cursor: pointer">
            <q-img @click="img5Grande = true" :src="img5" alt="img" style="height: 100%; width: 100%"/>
            <q-dialog v-model="img5Grande">
              <div style="height: auto; width: 100%; max-width: 1202px; overflow: hidden;">
                <q-img @click="img5Grande = false" :src="img1x5" alt="img"
                       style="height: auto; width: 100%; cursor: pointer"/>
              </div>
            </q-dialog>
          </div>
          <div class="col q-pa-md" style="cursor: pointer">
            <q-img @click="img6Grande = true" :src="img6" alt="img" style="height: 100%; width: 100%"/>
            <q-dialog v-model="img6Grande">
              <div style="height: auto; width: 100%; max-width: 1202px; overflow: hidden;">
                <q-img @click="img6Grande = false" :src="img1x6" alt="img"
                       style="height: auto; width: 100%; cursor: pointer"/>
              </div>
            </q-dialog>
          </div>
        </div>
        <div class="row col-12">
          <div class="col q-pa-md" style="cursor: pointer">
            <q-img @click="img7Grande = true" :src="img7" alt="img" style="height: 100%; width: 100%"/>
            <q-dialog v-model="img7Grande">
              <div style="height: auto; width: 100%; max-width: 1202px; overflow: hidden;">
                <q-img @click="img7Grande = false" :src="img1x7" alt="img"
                       style="height: auto; width: 100%; cursor: pointer"/>
              </div>
            </q-dialog>
          </div>
          <div class="col q-pa-md" style="cursor: pointer">
            <q-img @click="img8Grande = true" :src="img8" alt="img" style="height: 100%; width: 100%"/>
            <q-dialog v-model="img8Grande">
              <div style="height: auto; width: 100%; max-width: 1202px; overflow: hidden;">
                <q-img @click="img8Grande = false" :src="img1x8" alt="img"
                       style="height: auto; width: 100%; cursor: pointer"/>
              </div>
            </q-dialog>
          </div>
          <div class="col q-pa-md" style="cursor: pointer">
            <q-img @click="img10Grande = true" :src="img10" alt="img" style="height: 100%; width: 100%"/>
            <q-dialog v-model="img10Grande">
              <div style="height: auto; width: 100%; max-width: 1202px; overflow: hidden;">
                <q-img @click="img10Grande = false" :src="img1x10" alt="img"
                       style="height: auto; width: 100%; cursor: pointer"/>
              </div>
            </q-dialog>
          </div>
        </div>
        <div class="row col-12">
          <div class="col q-pa-md" style="cursor: pointer">
            <q-img @click="img11Grande = true" :src="img11" alt="img" style="height: 100%; width: 100%"/>
            <q-dialog v-model="img11Grande">
              <div style="height: auto; width: 100%; max-width: 1202px; overflow: hidden;">
                <q-img @click="img11Grande = false" :src="img1x11" alt="img"
                       style="height: auto; width: 100%; cursor: pointer"/>
              </div>
            </q-dialog>
          </div>
          <div class="col q-pa-md" style="cursor: pointer">
            <q-img @click="img12Grande = true" :src="img12" alt="img" style="height: 100%; width: 100%"/>
            <q-dialog v-model="img12Grande">
              <div style="height: auto; width: 100%; max-width: 1202px; overflow: hidden;">
                <q-img @click="img12Grande = false" :src="img1x12" alt="img"
                       style="height: auto; width: 100%; cursor: pointer"/>
              </div>
            </q-dialog>
          </div>
        </div>
      </div>
      <div class="col-12" id="servicos" style="margin-top: 100px">
        <div class="row col-12 items-center">
          <div class="text-blue-4" style="font-size: 46px; font-weight: bold; padding-left: 30px">
            CONTATO
          </div>
          <div class="col" style="padding-left: 20px; padding-right: 20px;">
            <div style="height: 5px; background-color: #ccc; width: 100%;"></div>
          </div>
        </div>
        <div class="row col-12">
          <div class="col-12 text-center" style="font-size: 20px">
            Av. Eugênio Fischer, 300 - Cing, Guarujá - SP, 11420-730
          </div>
          <div class="row col-12 justify-center items-center text-center" style="font-size: 20px; margin-top: 10px">
            <i class="fab fa-whatsapp" style="font-size: 24px; color: green; padding-right: 10px"></i>
            (13) 97405-2840
          </div>
          <div class="row col-12 justify-center items-center text-center" style="font-size: 20px; margin-top: 10px">
            <i class="fab fa-whatsapp" style="font-size: 24px; color: green; padding-right: 10px"></i>
            (13) 99664-5670
          </div>
          <div class="row col-12 justify-center items-center text-center" style="font-size: 20px; margin-top: 10px">
            <i class="fab fa-whatsapp" style="font-size: 24px; color: green; padding-right: 10px"></i>
            (13) 99719-1309
          </div>
        </div>
      </div>
      <div class="col-12" id="localizacao" style="margin-top: 100px">
        Localizacao
      </div>
    </div>
    <div>
    </div>
  </q-layout>
</template>

<script setup>
import '@fortawesome/fontawesome-free/css/all.css';
import logo from '/public/images/logo.png'
import sobrenos from '/public/images/sobrenos.png'
import video from '/public/images/video.mp4'
import img1 from '/public/images/1.jpg'
import img2 from '/public/images/2.jpg'
import img3 from '/public/images/3.jpg'
import img4 from '/public/images/4.jpg'
import img5 from '/public/images/5.jpg'
import img6 from '/public/images/6.jpg'
import img7 from '/public/images/7.jpg'
import img8 from '/public/images/8.jpg'
import img10 from '/public/images/10.jpg'
import img11 from '/public/images/11.jpg'
import img12 from '/public/images/12.jpg'
import img1x1 from '/public/images/1.1.jpg'
import img1x2 from '/public/images/2.1.jpg'
import img1x3 from '/public/images/3.1.jpg'
import img1x4 from '/public/images/4.1.jpg'
import img1x5 from '/public/images/5.1.jpg'
import img1x6 from '/public/images/6.1.jpg'
import img1x7 from '/public/images/7.1.jpg'
import img1x8 from '/public/images/8.1.jpg'
import img1x10 from '/public/images/10.1.jpg'
import img1x11 from '/public/images/11.1.jpg'
import img1x12 from '/public/images/12.1.jpg'
import {ref} from "vue";

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

const img1Grande = ref(false)
const img2Grande = ref(false)
const img3Grande = ref(false)
const img4Grande = ref(false)
const img5Grande = ref(false)
const img6Grande = ref(false)
const img7Grande = ref(false)
const img8Grande = ref(false)
const img9Grande = ref(false)
const img10Grande = ref(false)
const img11Grande = ref(false)
const img12Grande = ref(false)

function abrirWhatsApp(numero) {
  const mensagem = encodeURIComponent('Olá, gostaria de solicitar um orçamento.');
  const url = `https://wa.me/${numero}?text=${mensagem}`;
  window.open(url, '_blank');
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
