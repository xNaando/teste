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
              A W.E. Serviços Náuticos é uma empresa especializada em pintura e reforma de embarcações, localizada em
              Guarujá, SP. Com mais de 12 anos de experiência no setor, nossa missão é proporcionar aos nossos clientes
              serviços de
              alta qualidade, que garantam a durabilidade, segurança e beleza de suas embarcações. Contamos com uma
              equipe altamente capacitada, dedicada e comprometida em atender às necessidades de cada cliente,
              oferecendo soluções personalizadas para cada tipo de embarcação.
            </div>
            <div class="col-12">
              Trabalhamos com pintura, manutenção, reparos estruturais e reformas completas, utilizando materiais de
              primeira linha e tecnologia de ponta para garantir o melhor acabamento. Nossa infraestrutura é moderna e
              adequada para atender embarcações de diversos portes, garantindo agilidade e eficiência em cada projeto.
              Além disso, possuímos um atendimento personalizado, com foco na excelência e na satisfação total dos
              nossos clientes.
            </div>
            <div class="col-12">
              Na W.E. Serviços Náuticos, prezamos pela transparência e pelo comprometimento, proporcionando um trabalho
              bem-feito e com alto padrão de qualidade. Se você busca serviços especializados e confiança, a W.E. é a
              escolha certa para cuidar da sua embarcação com o profissionalismo que ela merece.
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
        <div class="row col-12 justify-center" style="margin-top: 30px">
          <div class="col">
            <video
              class="no-margin no-padding"
              :src="v1"
              autoplay
              loop
              muted
              playsinline
              style="height: 500px; width: 100%;"
            ></video>
          </div>
          <div class="col">
            <video
              class="no-margin no-padding"
              :src="v2"
              autoplay
              loop
              muted
              playsinline
              style="height: 500px; width: 100%;"
            ></video>
          </div>
          <div class="col">
            <video
              class="no-margin no-padding"
              :src="v3"
              autoplay
              loop
              muted
              playsinline
              style="height: 500px; width: 100%;"
            ></video>
          </div>
          <div class="col">
            <video
              class="no-margin no-padding"
              :src="v4"
              autoplay
              loop
              muted
              playsinline
              style="height: 500px; width: 100%;"
            ></video>
          </div>
          <div class="col">
            <video
              class="no-margin no-padding"
              :src="v5"
              autoplay
              loop
              muted
              playsinline
              style="height: 500px; width: 100%;"
            ></video>
          </div>
        </div>
        <div class="row col-12 justify-center">
          <div class="col">
            <video
              class="no-margin no-padding"
              :src="v6"
              autoplay
              loop
              muted
              playsinline
              style="height: 500px; width: 100%;"
            ></video>
          </div>
          <div class="col">
            <video
              class="no-margin no-padding"
              :src="v7"
              autoplay
              loop
              muted
              playsinline
              style="height: 500px; width: 100%;"
            ></video>
          </div>
          <div class="col">
            <video
              class="no-margin no-padding"
              :src="v8"
              autoplay
              loop
              muted
              playsinline
              style="height: 500px; width: 100%;"
            ></video>
          </div>
          <div class="col">
            <video
              class="no-margin no-padding"
              :src="v9"
              autoplay
              loop
              muted
              playsinline
              style="height: 500px; width: 100%;"
            ></video>
          </div>
          <div class="col">
            <video
              class="no-margin no-padding"
              :src="v10"
              autoplay
              loop
              muted
              playsinline
              style="height: 500px; width: 100%;"
            ></video>
          </div>
        </div>
      </div>
      <div class="col-12" id="contato" style="margin-top: 50px">
        <div class="row col-12 items-center">
          <div class="text-blue-4" style="font-size: 46px; font-weight: bold; padding-left: 30px">
            CONTATO
          </div>
          <div class="col" style="padding-left: 20px; padding-right: 20px;">
            <div style="height: 5px; background-color: #ccc; width: 100%;"></div>
          </div>
        </div>
        <div class="row col-12 items-center" style="margin-top: 30px; margin-left: 70px">
          <div class="col-12 text-center" style="margin-bottom: -100px">
            <div class="col-12 text-blue-4" style="font-size: 40px; font-weight: bold">
              Deseja obter um orçamento?
            </div>
            <div class="col-12" style="font-size: 40px; font-weight: bold; color: #203884">
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
import v1 from '/public/images/v1.mp4'
import v2 from '/public/images/v2.mp4'
import v3 from '/public/images/v3.mp4'
import v4 from '/public/images/v4.mp4'
import v5 from '/public/images/v5.mp4'
import v6 from '/public/images/v6.mp4'
import v7 from '/public/images/v7.mp4'
import v8 from '/public/images/v8.mp4'
import v9 from '/public/images/v9.mp4'
import v10 from '/public/images/v10.mp4'
import contato from '/public/images/contato.json'
import seta from '/public/images/seta.json'
import {ref} from "vue";

const navigateTo = (section) => {
  if (section === 'home') {
    window.scrollTo({top: 0, behavior: 'smooth'});
  } else {
    const element = document.getElementById(section);
    if (element) {
      const offset = 80; // Define a margem de 70px
      const elementPosition = element.getBoundingClientRect().top + window.scrollY - offset;
      window.scrollTo({top: elementPosition, behavior: 'smooth'});
    }
  }
}

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
