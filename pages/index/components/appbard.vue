<template>
  <v-app>
    <v-app-bar :elevation="2">
      <template v-slot:prepend>
        <v-app-bar-nav-icon></v-app-bar-nav-icon>
      </template>

      <v-app-bar-title @click="gotostar" class="myevent">MyEvent</v-app-bar-title>
      <v-app-bar-title @click="gotoorg"  class="prod_serv">Organiza tu evento</v-app-bar-title>
      <template v-slot:append>
        <v-btn icon="mdi-heart" @click="toggleComments"></v-btn>
        <v-text-field
        v-model="search"
        append-icon="mdi-magnify"
        label="Buscar"
        single-line
        hide-details
        class="Buscar"
        ></v-text-field> 
      </template>
    </v-app-bar>
<hero/>
    <div v-if="showComments" class="comments-container">
      <Comments
        v-for="(comment, index) in comments"
        :key="index"
        :nombredeusuario="comment.nombredeusuario"
        :comentario="comment.comentario"
        :visible="showComments"
      />
    </div>
  </v-app>
</template>

<script setup>
import { ref } from 'vue';
import hero from './hero.vue';
import Comments from './comments.vue';

const gotostar = () => {
  window.location.href = '/';
}
const gotopro = () =>  {
    window.location.href ='/products';
}
const showComments = ref(false);
const comments = ref([
  { nombredeusuario: '@vafer._.15', comentario: 'Este es el primer comentario.' },
  { nombredeusuario: '@facentejazz', comentario: 'Este es el segundo comentario.' },
  { nombredeusuario: '@jhosi_anteqra', comentario: 'Este es el tercer comentario.' },
  {nombredeusuario:'@ale._.mauri' , comentario: 'Muy bueno el servicio'}
]);

const toggleComments = () => {
  showComments.value = !showComments.value;
}
const search = ref('');

const gotoorg = () => {
  window.location.href = '/organiza'
}
</script>

<style>
.myevent {
  text-align: center;
  font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
  cursor: pointer;
  color: #ffffff;
  background-color: #73f0eb;
  margin-right: 20px;
  margin-left: 100px;
  border-radius: 10px;
}

.comments-container {
  margin-right: 100px;
  margin-left: 1095px;
  margin-top:-650px ;
}
.Buscar{
  width: 185px;
}
.prod_serv{
  text-align: center;
  margin-right: 30px;
  cursor: pointer;
  font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
  color: #ffffff;
  background-color: #ffa158;
  border-radius: 10px;
}
</style>
