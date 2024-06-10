<template>
    <v-footer
      class="color_b text-center  flex-column"
   >
      <div>
        <v-btn
          v-for="icon in icons"
          :key="icon"
          :icon="icon"
          class="mx-4"
          variant="text"
        ></v-btn>
      </div>
  
      <div class="pt-0">
        MyEventBO, el lugar donde tu puedes confiar para hacer las mejores fiestas y evetos y sorprender a todos tus amigos y familia. 
        <br>    ©CopyRight 2024
      </div>
  
      <v-divider></v-divider>
  
      <div>
        {{ new Date().getFullYear() }} — <strong>MyEventBO</strong>
      </div>
    </v-footer>
  </template>

<script>
  export default {
    data: () => ({
      icons: [
        'mdi-facebook',
        'mdi-twitter',
        'mdi-linkedin',
        'mdi-instagram',
      ],
    }),
  }
</script>


