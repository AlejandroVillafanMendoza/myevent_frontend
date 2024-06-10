<template>
    <v-container>
      <div class="aboutus">  <h1>Sobre Nosotros</h1></div>

<v-row>

    <v-col cols="12" xl="6" lg="6" md="6" sm="12" xs="12"> 
        <img src="/public/img/MyEvent_logo.png" alt="Not Found" width="400px" height="400px" class="img_1">
    </v-col>

    <v-col cols="12" xl="6" lg="6" md="6" sm="12" xs="12" class="texto1">
        "¡Bienvenido a nuestra plataforma de organización de eventos! Somos tu aliado 
        perfecto para convertir cualquier ocasión en un momento inolvidable. 
        Con nuestra amplia gama de herramientas intuitivas y personalizables, 
        planificar desde pequeñas reuniones hasta grandes celebraciones nunca ha sido tan sencillo. 
        Navega por nuestra interfaz fácil de usar, donde podrás encontrar todo lo que necesitas: 
        desde la selección del lugar ideal y la gestión de invitados hasta la coordinación de servicios 
        adicionales como catering y entretenimiento. Además, nuestro equipo de expertos está siempre disponible 
        para brindarte asesoramiento y apoyo en cada paso del proceso. Con nosotros, cada detalle está cuidadosamente atendido, 
        permitiéndote concentrarte en disfrutar del evento junto a tus invitados. 
        Únete a nuestra comunidad de organizadores de eventos 
        y haz realidad tus sueños de celebración. 
        Empieza a crear recuerdos inolvidables hoy mismo!"

    </v-col>
  
        

</v-row>
    </v-container>

</template>

<script setup>

</script>

<style>
.texto1{
    text-transform: uppercase;
    text-align: justify;
    margin-left: -30px;

}
.aboutus{
     text-align: center;
    text-transform: uppercase;
    font-family: Arial, Helvetica, sans-serif;
    font-size: 30px;
    font-weight: 700;
    color:#73f0eb;
}
.img_1{
    align-items: center;
    margin-left: 150px;
}
</style>