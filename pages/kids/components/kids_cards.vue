
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
            <v-btn color="orange-lighten-2" text>Explore</v-btn>
            <v-spacer></v-spacer>
          </v-card-actions>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>

<script setup>
const items = [
{ titulo: 'Decorado Sencillo', 
  subtitulo: '100 BOB', 
  text: 'Decorado sencillo con globos (colores a eleccion)', 
  image: '/img/kids_cards/card_kid_1.jpg' },


{ titulo: 'Decorado Tematico', 
  subtitulo: '150 BOB', 
  text: 'Decorado Tematico (Tematica a Eleccion)', 
  image: '/img/kids_cards/card_kid_2.jpg' },

{ titulo: 'Candy Bar Simple', 
  subtitulo: '250 BOB', 
  text: 'Varieda de ducel para 15 personas', 
  image: '/img/kids_cards/card_kid_3.jpg' },

  { titulo: 'Candy Bar Premium', 
  subtitulo: '350 BOB', 
  text: 'Varieda de ducel para 30 personas', 
  image: '/img/kids_cards/card_kid_4.jpg' },

  { titulo: 'Botargas', 
  subtitulo: '100 BOB / hora', 
  text: 'Alquieler de Botargas para animar tu fiesta', 
  image: '/img/kids_cards/card_kid_5.jpg' },

  { titulo: 'Payasitos', 
  subtitulo: '150 BOB / hora', 
  text: 'La divercion no va a faltar con nuestros increibles payasitos', 
  image: '/img/kids_cards/card_kid_6.jpg' },
]
</script>

