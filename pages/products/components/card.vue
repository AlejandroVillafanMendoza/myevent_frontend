<template>
  <v-container>
    <v-row>
      <v-col
        v-for="(item, index) in items"
        :key="index"
        cols="12"
        md="4"
      >
        <v-card class="mx-auto" max-width="400">
          <v-img :src="item.image" height="200px" cover></v-img>
          <v-card-title>{{ item.titulo }}</v-card-title>
          <v-card-subtitle>{{ item.subtitulo }}</v-card-subtitle>
          <v-card-text>{{ item.text }}</v-card-text>
          <v-card-actions>
            <v-btn color="orange-lighten-2" text>Agregar</v-btn>
            <v-spacer></v-spacer>
          </v-card-actions>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>

<script setup>
const items = [

  { titulo: 'Ositos de Goma', 
  subtitulo: '10$', 
  text: '', 
  image: '/img/productos_img/candy_1.jpg' },

  { titulo: 'Bolsa grande Doritos', 
  subtitulo: '10$', 
  text: '', 
  image: '/img/productos_img/candy_2.jpg' },

  { titulo: 'Sprite 3L', 
  subtitulo: '10$', 
  text: '', 
  image: '/img/productos_img/candy_3.jpg' },

  { titulo: 'Cola-Cola 3L', 
  subtitulo: '10$', 
  text: '', 
  image: '/img/productos_img/candy_4.jpg' },

  { titulo: 'Fanta 3L', 
  subtitulo: '10$', 
  text: '', 
  image: '/img/productos_img/candy_6.jpg' },

  { titulo: 'Bolsa Grande Malvabiscos', 
  subtitulo: '10$', 
  text: '', 
  image: '/img/productos_img/candy_5.jpg' },


  { titulo: 'Caja de Sublime', 
  subtitulo: '10$', 
  text: '', 
  image: '/img/productos_img/candy_7.jpg' },

  { titulo: 'Bolsa Grade Gomitas de Zandia ', 
  subtitulo: '10$', 
  text: '', 
  image: '/img/productos_img/candy_8.jpg' },

  { titulo: 'Bolsa Grande Chupetes', 
  subtitulo: '10$', 
  text: 'Texto 1', 
  image: '/img/productos_img/candy_9.jpg' },

  { titulo: 'Bolsa Grande de Gomitas Ladrillos', 
  subtitulo: '10$', 
  text: '', 
  image: '/img/productos_img/candy_10.jpg' },

  { titulo: 'Bolsa grande Papas Fritas', 
  subtitulo: '10$', 
  text: '', 
  image: '/img/productos_img/candy_11.jpg' },

{ titulo: 'Bolsa Grande TAKIS', 
  subtitulo: '15$', 
  text: '', 
  image: '/img/productos_img/candy_12.jpg' },

{ titulo: 'hallwringhts', 
  subtitulo: '130$ por plato', 
  text: 'Servicio Catering', 
  image: '/img/productos_img/Catering_1.jpg' },

  { titulo: 'Pasion Criolla', 
  subtitulo: '30$ por plato', 
  text: 'Servicio de Catering', 
  image: '/img/productos_img/Catering_2.jpg' },

  { titulo: 'Rimini', 
  subtitulo: '30$ por plato', 
  text: 'Servio de Catering', 
  image: '/img/productos_img/Catering_3.jpg' },

  { titulo: 'Cortina Dorada', 
  subtitulo: '5$ c/u', 
  text: '', 
  image: '/img/productos_img/Cornita_1.jpg' },

  { titulo: 'Cortina Verde', 
  subtitulo: '5$', 
  text: '', 
  image: '/img/productos_img/Cornita_3.jpg' },

  { titulo: 'Cortina Naranja', 
  subtitulo: '5$', 
  text: '', 
  image: '/img/productos_img/Cornita_4.jpg' },

  { titulo: 'Cortina Azul', 
  subtitulo: '5$', 
  text: '', 
  image: '/img/productos_img/Cornita_5.jpg' },

  { titulo: 'Paquete Globos Rosados', 
  subtitulo: '10$', 
  text: '', 
  image: '/img/productos_img/Globos_1.jpg' },

  { titulo: 'Paquete Globos Azules', 
  subtitulo: '10$', 
  text: '', 
  image: '/img/productos_img/Globos_2.jpg' },

  { titulo: 'Paquete Globos Rojos', 
  subtitulo: '10$', 
  text: '', 
  image: '/img/productos_img/Globos_3.jpg' },

  { titulo: 'Paquete Globos Verdes', 
  subtitulo: '10$', 
  text: '', 
  image: '/img/productos_img/Globos_4.jpg' },

  { titulo: 'Paquete Globos Varios Colores', 
  subtitulo: '11$', 
  text: 'Rojo, Azul, Verde, Rosado, amarillo', 
  image: '/img/productos_img/Globos_5.jpg' },

  { titulo: 'Sound Record Party', 
  subtitulo: '10$ / h', 
  text: 'Servicio de Amplificación', 
  image: '/img/productos_img/ampli_1.jpg' },

  { titulo: 'Music Party', 
  subtitulo: '15$ / h', 
  text: 'Servicio de Amplificación', 
  image: '/img/productos_img/ampli_2.jpg' },

  { titulo: 'Maquina de Humo', 
  subtitulo: '10$ / hora', 
  text: 'Servicios', 
  image: '/img/productos_img/ampli_3.jpg' },

  { titulo: 'Maquina de Burbujas', 
  subtitulo: '10$ / h', 
  text: 'Servicios', 
  image: '/img/productos_img/ampli_4.jpg' },

  { titulo: 'Party Led', 
  subtitulo: '10$ / h', 
  text: 'Servicios de Ilumunacion', 
  image: '/img/productos_img/ampli_5.jpg' },

  { titulo: 'Light&Night', 
  subtitulo: '15$ / h', 
  text: 'Servicio de Iluminacion', 
  image: '/img/productos_img/ampli_6.jpg' },

  
]
</script>

