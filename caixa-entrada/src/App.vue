<template>
  <v-app>
      <v-app theme="dark">
        <v-navigation-drawer v-model="isDrawerOpen">
          <v-card> 
          <v-menu>
            <template #activator="{ props }"> 
        <v-avatar size="68" v-bind="props" class="mx-12" >
          <v-img 
          cover 
          src="https://i.pinimg.com/236x/9c/33/2e/9c332e390ef163a111402497c28acc0d.jpg" ></v-img>
        </v-avatar>
      </template>
    </v-menu>
   <v-list-subheader class="ml-4 ">blackwid@gmail.com</v-list-subheader>
  </v-card>
      <v-list-item prepend-icon="mdi-mail">Caixa de entrada</v-list-item> 
      <v-list-item prepend-icon="mdi-send">Enviar</v-list-item>
      <v-list-item prepend-icon="mdi-delete">Lixo</v-list-item>
    </v-navigation-drawer> 
    <v-app-bar :elevation="3" >
      <v-app-bar-nav-icon @click="isDrawerOpen = !isDrawerOpen"></v-app-bar-nav-icon>
      <v-app-bar-title>Mensages</v-app-bar-title>
    </v-app-bar>

      <v-main>
        <v-card class=" pa-6 ma-5 w-70 h-70" >
        <v-list lines="two">
     <v-list-item-subtitle >Hoje</v-list-item-subtitle>
  <v-list-item
    prepend-avatar = "https://i.pinimg.com/736x/fb/13/41/fb1341531be816dc9fc5cdffbe28c38e.jpg"
    title="Steve Rogers "
    template >
          <span class="font-weight-bold">Mensagem importante!!</span> &mdash; Oi Nath, preciso conversar com você, é urgente! Preciso que venha a torre dos Vingadores 
</v-list-item>
<v-divider inset></v-divider>
  </v-list>

  <v-list lines="two">
      <v-list-item 
        prepend-avatar = " https://i.pinimg.com/736x/a4/fe/6f/a4fe6fdafcb95b9c14cb6bc90ef54cb7.jpg"
        title="Tony Stark"
        template >
          <span class="font-weight-bold">A coisa ficou verde! quer dizer... *feia</span> &mdash;
        Mas notícias, o grandão fugiu, por favor me diga que ele está com você. Se não estamos fritos!
      </v-list-item>
      
      <v-divider inset></v-divider>
       </v-list>

       <v-list lines="two">
      <v-list-item 
        prepend-avatar = " https://64.media.tumblr.com/e80b00fb83c8f177576782ec12aeae26/tumblr_pvdwl4NBP31t4rhclo4_400.png"
        title="Thor"
        template >
          <span class="font-weight-bold">Onde você está???</span> &mdash; Natasha, o Steve e o Tony estão te procurando 
      </v-list-item>
      
      <v-divider inset></v-divider>
       </v-list>
       
       <v-list lines="two">
         <v-list-item 
         prepend-avatar = " https://2img.net/u/1215/51/18/82/avatars/238-37.jpg"
         title="Clint Barton"
         template >
          <span class="font-weight-bold">Estamos procurando o Hulk </span> &mdash; Nath, o Tony e o Steve já falaram com você?, é sobre o Bruce 
        </v-list-item>
      </v-list>
      <v-divider inset  class="border-opacity-75"></v-divider>
    
      <v-list lines="two">
        <v-list-item-subtitle class=" pt-10">Ontem</v-list-item-subtitle>
        <v-list> 
          <v-list-item 
          prepend-avatar = "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRABrMw645CTGaHG_OHRpSce6c35119ygJTgyrzu0Fx82aVb_Oyc23kUd7J6SltxqjnpQw&usqp=CAU"
          title="Nick Fury"
          template >
          <span class="font-weight-bold">Preciso encontrar você</span> &mdash; Agente Romanoff temos alguns assuntos pendentes, espero que esteja lembrada
        </v-list-item>
      </v-list>
      <v-divider inset></v-divider>

      <v-list> 
          <v-list-item 
          prepend-avatar = "https://i.pinimg.com/474x/20/8e/f2/208ef2b8508379a323ab3dcd8feb1395.jpg"
          title="Yelena"
          template >
          <span class="font-weight-bold">Lembra de Mim?</span> &mdash; Adivinha quem voltou...
        </v-list-item>
      </v-list>
      <v-divider inset></v-divider>

      <v-list lines="two"> 
      <v-list-item 
      prepend-avatar = " https://i.pinimg.com/736x/d5/e3/a8/d5e3a8559fac7755f2f1a817270cfecc.jpg"
      title="Bruce Benner"
      template >
          <span class="font-weight-bold">Posso ir aí ??</span> &mdash; Nath eu preciso te ver, as coisas estão saindo do meu controle, não aguento mais!
     </v-list-item>
    </v-list>
    <v-divider inset></v-divider>

      <v-list lines="two"> 
      <v-list-item 
      prepend-avatar = "https://w7.pngwing.com/pngs/560/211/png-transparent-iron-man-captain-america-phil-coulson-s-h-i-e-l-d-marvel-cinematic-universe-iron-man-marvel-avengers-assemble-avengers-logo.png"
      title="S.H.I.E.L.D"
      template >
          <span class="font-weight-bold"> ~ Reunião as 23:00 Hs</span> &mdash; Agente Romanoff esta é uma mensagem pra marcar sua presença hoje a noite 
     </v-list-item>
    </v-list>
  </v-list>
      
      
       
      
       
       
       
       
       
       
      </v-card>
      </v-main>
    </v-app>
  </v-app>
</template>

<script setup>

   

import {ref} from 'vue';
const isDrawerOpen = ref (false)
</script>
