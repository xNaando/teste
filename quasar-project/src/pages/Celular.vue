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
    <div class="row col-12" style="margin-top: 70px">
      <div class="col-12" id="home">
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
      <div class="row col-12" id="sobre-nos" style="margin-top: 10px">
        <div class="row col-12 items-center">
          <div class="text-blue-4" style="padding-left: 10px; font-size: 32px; font-weight: bold;">
            SOBRE NÓS
          </div>
        </div>
        <div class="col-12">
          <q-img :src="sobrenos" alt="img" style="height: auto; width: 100%"/>
        </div>
        <div class="row col-12">
          <div class="row col-12" style="font-size: 14px; margin-top: 10px; padding-inline: 10px">
            <div class="col-12">
              A W.E. Serviços Náuticos é uma empresa especializada em pintura e reforma de embarcações, localizada em
              Guarujá, SP. Com mais de 12 anos de experiência no setor, nossa missão é proporcionar aos nossos clientes
              serviços de
              alta qualidade, que garantam a durabilidade, segurança e beleza de suas embarcações. Contamos com uma
              equipe altamente capacitada, dedicada e comprometida em atender às necessidades de cada cliente,
              oferecendo soluções personalizadas para cada tipo de embarcação.
            </div>
            <div class="col-12" style="margin-top: 10px">
              Trabalhamos com pintura, manutenção, reparos estruturais e reformas completas, utilizando materiais de
              primeira linha e tecnologia de ponta para garantir o melhor acabamento. Nossa infraestrutura é moderna e
              adequada para atender embarcações de diversos portes, garantindo agilidade e eficiência em cada projeto.
              Além disso, possuímos um atendimento personalizado, com foco na excelência e na satisfação total dos
              nossos clientes.
            </div>
            <div class="col-12" style="margin-top: 10px">
              Na W.E. Serviços Náuticos, prezamos pela transparência e pelo comprometimento, proporcionando um trabalho
              bem-feito e com alto padrão de qualidade. Se você busca serviços especializados e confiança, a W.E. é a
              escolha certa para cuidar da sua embarcação com o profissionalismo que ela merece.
            </div>
          </div>
          <div class="col-12 text-blue-4"
               style="padding-inline: 10px; font-size: 18px; margin-top: 30px; font-weight: bold;">
            FAZER DOS SEUS MOMENTOS DE ESPORTE E LAZER NÁUTICO UMA EXPERIÊNCIA AGRADÁVEL É NOSSA OBRIGAÇÃO!
          </div>
        </div>
      </div>
      <div class="row col-12" id="servicos" style="margin-top: 30px">
        <div class="row col-12 items-center">
          <div class="text-blue-4" style="font-size: 32px; font-weight: bold; padding-left: 10px">
            NOSSOS SERVIÇOS
          </div>
        </div>
        <div class="row col-12 text-white" style="font-size: 15px">
          <div class="col-12 bg-blue-4 q-pa-sm">
            01. Reparos em fibra de vidro
          </div>
          <div class="col-12" style="height: 2px"/>
          <div class="col-12 bg-blue-4 q-pa-sm">
            02. Tratamento de Osmose
          </div>
          <div class="col-12" style="height: 2px"/>
          <div class="col-12 bg-blue-4 q-pa-sm">
            03. Pintura e retoque em gel coats
          </div>
          <div class="col-12" style="height: 2px"/>
          <div class="col-12 bg-blue-4 q-pa-sm">
            04. Letreiros
          </div>
          <div class="col-12" style="height: 2px"/>
          <div class="col-12 bg-blue-4 q-pa-sm">
            05. Pintura de faixas personalizadas
          </div>
          <div class="col-12" style="height: 2px"/>
          <div class="col-12 bg-blue-4 q-pa-sm">
            06. Alongamento de plataforma
          </div>
          <div class="col-12" style="height: 2px"/>
          <div class="col-12 bg-blue-4 q-pa-sm">
            07. Troca de sicaflex
          </div>
          <div class="col-12" style="height: 2px"/>
          <div class="col-12 bg-blue-4 q-pa-sm">
            08. Polimento com espelhamento
          </div>
          <div class="col-12" style="height: 2px"/>
          <div class="col-12 bg-blue-4 q-pa-sm">
            09. Lixamento de Teka
          </div>
          <div class="col-12" style="height: 2px"/>
          <div class="col-12 bg-blue-4 q-pa-sm">
            10. Aplicação de tinta anti-crustante
          </div>
          <div class="col-12" style="height: 2px"/>
          <div class="col-12 bg-blue-4 q-pa-sm">
            11. Modificação estrutural
          </div>
          <div class="col-12" style="height: 2px"/>
          <div class="col-12 bg-blue-4 q-pa-sm">
            12. Aplicação de Propspeed
          </div>
          <div class="col-12" style="height: 2px"/>
          <div class="col-12 bg-blue-4 q-pa-sm">
            13. Fabricação de plataforma submergível
          </div>
          <div class="col-12" style="height: 2px"/>
          <div class="col-12 bg-blue-4 q-pa-sm">
            14. Fabricação de teka
          </div>
          <div class="col-12" style="height: 2px"/>
          <div class="col-12 bg-blue-4 q-pa-sm">
            15. Fabricação espaço gourmand
          </div>
          <div class="col-12" style="height: 2px"/>
          <div class="col-12 bg-blue-4 q-pa-sm">
            16. Fabricação HARD TOP
          </div>
        </div>
      </div>
      <div class="row col-12" id="pinturas-nauticas" style="margin-top: 30px">
        <div class="row col-12 items-center">
          <div class="text-blue-4" style="font-size: 32px; font-weight: bold; padding-left: 10px">
            PINTURAS NÁUTICAS
          </div>
        </div>
        <div class="row col-12">
          <div class="col q-pa-xs" style="cursor: pointer">
            <q-img @click="img1Grande = true" :src="img1" alt="img" style="height: 100%; width: 100%"/>
            <q-dialog v-model="img1Grande">
              <div style="height: auto; width: 100%; max-width: 1202px; overflow: hidden;">
                <q-img @click="img1Grande = false" :src="img1x1" alt="img"
                       style="height: auto; width: 100%; cursor: pointer"/>
              </div>
            </q-dialog>
          </div>
          <div class="col q-pa-xs" style="cursor: pointer">
            <q-img @click="img2Grande = true" :src="img2" alt="img" style="height: 100%; width: 100%"/>
            <q-dialog v-model="img2Grande">
              <div style="height: auto; width: 100%; max-width: 1202px; overflow: hidden;">
                <q-img @click="img2Grande = false" :src="img1x2" alt="img"
                       style="height: auto; width: 100%; cursor: pointer"/>
              </div>
            </q-dialog>
          </div>
        </div>
        <div class="row col-12">
          <div class="col q-pa-xs" style="cursor: pointer">
            <q-img @click="img3Grande = true" :src="img3" alt="img" style="height: 100%; width: 100%"/>
            <q-dialog v-model="img3Grande">
              <div style="height: auto; width: 100%; max-width: 1202px; overflow: hidden;">
                <q-img @click="img3Grande = false" :src="img1x3" alt="img"
                       style="height: auto; width: 100%; cursor: pointer"/>
              </div>
            </q-dialog>
          </div>
          <div class="col q-pa-xs" style="cursor: pointer">
            <q-img @click="img4Grande = true" :src="img4" alt="img" style="height: 100%; width: 100%"/>
            <q-dialog v-model="img4Grande">
              <div style="height: auto; width: 100%; max-width: 1202px; overflow: hidden;">
                <q-img @click="img4Grande = false" :src="img1x4" alt="img"
                       style="height: auto; width: 100%; cursor: pointer"/>
              </div>
            </q-dialog>
          </div>
        </div>
        <div class="row col-12">
          <div class="col q-pa-xs" style="cursor: pointer">
            <q-img @click="img5Grande = true" :src="img5" alt="img" style="height: 100%; width: 100%"/>
            <q-dialog v-model="img5Grande">
              <div style="height: auto; width: 100%; max-width: 1202px; overflow: hidden;">
                <q-img @click="img5Grande = false" :src="img1x5" alt="img"
                       style="height: auto; width: 100%; cursor: pointer"/>
              </div>
            </q-dialog>
          </div>
          <div class="col q-pa-xs" style="cursor: pointer">
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
          <div class="col q-pa-xs" style="cursor: pointer">
            <q-img @click="img7Grande = true" :src="img7" alt="img" style="height: 100%; width: 100%"/>
            <q-dialog v-model="img7Grande">
              <div style="height: auto; width: 100%; max-width: 1202px; overflow: hidden;">
                <q-img @click="img7Grande = false" :src="img1x7" alt="img"
                       style="height: auto; width: 100%; cursor: pointer"/>
              </div>
            </q-dialog>
          </div>
          <div class="col q-pa-xs" style="cursor: pointer">
            <q-img @click="img8Grande = true" :src="img8" alt="img" style="height: 100%; width: 100%"/>
            <q-dialog v-model="img8Grande">
              <div style="height: auto; width: 100%; max-width: 1202px; overflow: hidden;">
                <q-img @click="img8Grande = false" :src="img1x8" alt="img"
                       style="height: auto; width: 100%; cursor: pointer"/>
              </div>
            </q-dialog>
          </div>
        </div>
        <div class="row col-12">
          <div class="col q-pa-xs" style="cursor: pointer">
            <q-img @click="img10Grande = true" :src="img10" alt="img" style="height: 100%; width: 100%"/>
            <q-dialog v-model="img10Grande">
              <div style="height: auto; width: 100%; max-width: 1202px; overflow: hidden;">
                <q-img @click="img10Grande = false" :src="img1x10" alt="img"
                       style="height: auto; width: 100%; cursor: pointer"/>
              </div>
            </q-dialog>
          </div>
          <div class="col q-pa-xs" style="cursor: pointer">
            <q-img @click="img11Grande = true" :src="img11" alt="img" style="height: 100%; width: 100%"/>
            <q-dialog v-model="img11Grande">
              <div style="height: auto; width: 100%; max-width: 1202px; overflow: hidden;">
                <q-img @click="img11Grande = false" :src="img1x11" alt="img"
                       style="height: auto; width: 100%; cursor: pointer"/>
              </div>
            </q-dialog>
          </div>
        </div>
        <div class="row col-12">
          <div class="col q-pa-xs" style="cursor: pointer">
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
      <div class="col-12" id="contato" style="margin-top: 30px">
        <div class="row col-12 items-center">
          <div class="text-blue-4" style="font-size: 32px; font-weight: bold; padding-left: 10px">
            CONTATO
          </div>
        </div>
        <div class="row col-12 items-center" style="margin-top: 30px; margin-left: 70px">
          <div class="col-12 text-center" style="margin-bottom: -100px">
            <div class="col-12 text-blue-4" style="font-size: 40px; font-weight: bold">
              Deseja obter um orçamento?
            </div>
            <div class="col-12" style="font-size: 40px; font-weight: bold">
              Entre em contato!
            </div>
          </div>
          <div class="row col-7 text-center items-center">
            <div class="col-6" id="lottie-container"/>
            <div class="col-6" id="lottie-container2"/>
          </div>
          <div class="col-5">
            <div class="row col-12 items-center" style="font-size: 20px; margin-top: 10px">
              <a
                href="https://www.google.com/maps/place/Av.+Eugênio+Fischer,+300+-+Cing,+Guarujá+-+SP,+11420-730"
                target="_blank"
                rel="noopener noreferrer"
                style="text-decoration: none; color: inherit"
              >
                <i class="fas fa-map-marker-alt" style="font-size: 24px; color: red; padding-right: 10px"></i>
                Av. Eugênio Fischer, 300 - Cing, Guarujá - SP, 11420-730
              </a>
            </div>
            <div
              class="row col-12 items-center"
              style="font-size: 20px; margin-top: 10px; cursor: pointer"
              @click="abrirWhatsApp('13974052840')"
            >
              <i class="fab fa-whatsapp" style="font-size: 24px; color: green; padding-right: 10px"></i>
              (13) 97405-2840
            </div>
            <div
              class="row col-12 items-center"
              style="font-size: 20px; margin-top: 10px; cursor: pointer"
              @click="abrirWhatsApp('13996645670')"
            >
              <i class="fab fa-whatsapp" style="font-size: 24px; color: green; padding-right: 10px"></i>
              (13) 99664-5670
            </div>
            <div
              class="row col-12 items-center"
              style="font-size: 20px; margin-top: 10px; cursor: pointer"
              @click="abrirWhatsApp('13997191309')"
            >
              <i class="fab fa-whatsapp" style="font-size: 24px; color: green; padding-right: 10px"></i>
              (13) 99719-1309
            </div>
            <div
              class="row col-12 items-center"
              style="font-size: 20px; margin-top: 10px; cursor: pointer"
              @click="abrirInstagram('w.e_servicosnauticos')"
            >
              <i class="fab fa-instagram" style="font-size: 24px; color: #E1306C; padding-right: 10px"></i>
              w.e_servicosnauticos
            </div>
          </div>
        </div>
      </div>
      <div class="col-12" id="localizacao" style="margin-top: 50px">
        <div class="row col-12 items-center">
          <div class="text-blue-4" style="font-size: 46px; font-weight: bold; padding-left: 30px">
            LOCALIZAÇÃO
          </div>
          <div class="col" style="padding-left: 20px; padding-right: 20px;">
            <div style="height: 5px; background-color: #ccc; width: 100%;"></div>
          </div>
        </div>
        <div class="row col-12 justify-center items-center text-center" style="margin-top: 50px">
          <iframe
            src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3657.819508282658!2d-46.24340698444323!3d-23.95793098448871!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x94ce03389eb90f0b%3A0x3f14a136ab96a979!2sAv.%20Eug%C3%AAnio%20Fischer%2C%20300%20-%20Cing%2C%20Guaruj%C3%A1%20-%20SP%2C%2011420-730!5e0!3m2!1sen!2sbr!4v1696781234567!5m2!1sen!2sbr"
            width="95%"
            height="600"
            style="border: 0;"
            allowfullscreen=""
            loading="lazy"
            referrerpolicy="no-referrer-when-downgrade"
          ></iframe>
        </div>
      </div>
    </div>
    <div class="row col-12 bg-blue-4 items-center justify-center text-center text-white"
         style="height: 70px; font-size: 16px; font-weight: 500; margin-top: 50px">
      <i class="fas fa-copyright" style="margin-right: 5px;"></i>
      W.E Serviços Náuticos - Todos os direitos reservados
    </div>
  </q-layout>
</template>

<script setup>
import '@fortawesome/fontawesome-free/css/all.css';
import {onMounted} from 'vue';
import lottie from 'lottie-web';
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
import contato from '/public/images/contato.json'
import seta from '/public/images/seta.json'
import {ref} from "vue";

const img1Grande = ref(false)
const img2Grande = ref(false)
const img3Grande = ref(false)
const img4Grande = ref(false)
const img5Grande = ref(false)
const img6Grande = ref(false)
const img7Grande = ref(false)
const img8Grande = ref(false)
const img10Grande = ref(false)
const img11Grande = ref(false)
const img12Grande = ref(false)

function abrirWhatsApp(numero) {
  const mensagem = encodeURIComponent('Olá, gostaria de solicitar um orçamento.');
  const url = `https://wa.me/${numero}?text=${mensagem}`;
  window.open(url, '_blank');
}

function abrirInstagram(username) {
  const url = `https://www.instagram.com/${username}`;
  window.open(url, '_blank');
}

onMounted(() => {
  lottie.loadAnimation({
    container: document.getElementById('lottie-container'), // Contêiner onde a animação será renderizada
    renderer: 'svg', // Formato da renderização
    loop: true, // Define se a animação será em loop
    autoplay: true, // Define se a animação será iniciada automaticamente
    animationData: contato, // Use os dados da animação diretamente
  });
  lottie.loadAnimation({
    container: document.getElementById('lottie-container2'), // Contêiner onde a animação será renderizada
    renderer: 'svg', // Formato da renderização
    loop: true, // Define se a animação será em loop
    autoplay: true, // Define se a animação será iniciada automaticamente
    animationData: seta, // Use os dados da animação diretamente
  });
});
</script>

<style scoped>
.q-header {
  padding: 10px 20px;
}

.q-btn {
  font-size: 16px;
  font-weight: 500;
}

#lottie-container {
  width: 400px; /* Largura do contêiner */
  height: 400px; /* Altura do contêiner */
}
</style>
