<template>
    <v-sheet class="mx-auto" width="500" elevation="10">
      <v-form ref="form">
        <h3 class="section-title">Información General del Evento</h3>
  
        <v-text-field
          v-model="eventName"
          :rules="eventNameRules"
          label="Nombre del evento"
          required
          class="custom-input"
        ></v-text-field>
  
        <v-text-field
          v-model="eventDate"
          :rules="eventDateRules"
          label="Fecha del evento"
          required
          class="custom-input"
        ></v-text-field>
  
        <v-text-field
          v-model="eventLocation"
          :rules="eventLocationRules"
          label="Ubicación del evento"
          required
          class="custom-input"
        ></v-text-field>
  
        <v-select
          v-model="eventType"
          :items="eventTypes"
          :rules="[v => !!v || 'El tipo de evento es requerido']"
          label="Tipo de evento"
          required
          class="custom-input"
        ></v-select>

        <v-textarea
          v-model="eventDescription"
          :rules="eventDescriptionRules"
          label="Descripción del evento"
          required
          class="custom-input"
        ></v-textarea>
  
        <h3 class="section-title">Información del Organizador</h3>
  
        <v-text-field
          v-model="fullName"
          :rules="fullNameRules"
          label="Nombre completo"
          required
          class="custom-input"
        ></v-text-field>
  
        <v-text-field
          v-model="email"
          :rules="emailRules"
          label="Correo electrónico"
          required
          class="custom-input"
        ></v-text-field>
  
        <v-text-field
          v-model="phoneNumber"
          :rules="phoneNumberRules"
          label="Número de teléfono"
          required
          class="custom-input"
        ></v-text-field>
  
        <v-text-field
          v-model="address"
          :rules="addressRules"
          label="Dirección"
          required
          class="custom-input"
        ></v-text-field>
  
        <div class="d-flex flex-column">
          <v-btn
            class="mt-4 custom-btn success-btn"
            block
            @click="validate"
          >
            Enviar Formulario
          </v-btn>
  
          <v-btn
            class="mt-4 custom-btn error-btn"
            block
            @click="reset"
          >
            Limpiar
          </v-btn>
  
        
        </div>
      </v-form>
    </v-sheet>
  </template>
  
  <script>
  export default {
    data: () => ({
      eventName: '',
      eventNameRules: [
        v => !!v || 'El nombre del evento es requerido',
      ],
      eventDate: '',
      eventDateRules: [
        v => !!v || 'La fecha y hora del evento son requeridos',
      ],
      eventLocation: '',
      eventLocationRules: [
        v => !!v || 'La ubicación del evento es requerida',
      ],
      eventDescription: '',
      eventDescriptionRules: [
        v => !!v || 'La descripción del evento es requerida',
      ],
      eventType: null,
      eventTypes: [
        'Bodas',
        'Cumpleaños',
        'Cumpleaños para niños',
        'Cumpleaños Tematico',
        'Cumpleaños Sorpresa',
        'Fiesta tematica',
        'Cena de gala',
        'Fiesta XV años',
        'Fiesta Navideña',
        'Fiesta de Añó Nuevo',
        'Fiesta de Hallowin',
        'Aniversario de Boda',
        'Otro'
      ],
      fullName: '',
      fullNameRules: [
        v => !!v || 'El nombre completo es requerido',
      ],
      email: '',
      emailRules: [
        v => !!v || 'El correo electrónico es requerido',
        v => /.+@.+\..+/.test(v) || 'El correo electrónico debe ser válido',
      ],
      phoneNumber: '',
      phoneNumberRules: [
        v => !!v || 'El número de teléfono es requerido',
      ],
      address: '',
      addressRules: [
        v => !!v || 'La dirección es requerida',
      ],
    }),
  
    methods: {
      async validate() {
        const { valid } = await this.$refs.form.validate()
  
        if (valid) alert('Gracias por llenar el formulario, te llegara un correo para poder empezar a ver mas detalles de tu evento')
      },
      reset() {
        this.$refs.form.reset()
      },
      resetValidation() {
        this.$refs.form.resetValidation()
      },
    },
  }
  </script>
  
  <style scoped>
  .section-title {
    color: #f8ffc0;
    font-size: 1.5rem;
    margin-bottom: 10px;
    background-color: #ffc0cb;
    border-radius: 12px;
    text-align: center;
  }
  
  .custom-input .v-input__control {
    background-color: #f8ffc0;
  }
  
  .custom-input .v-label {
    color: #11f1f1;
  }
  
  .custom-input .v-input__slot:before {
    border-color: #11f1f1;
  }
  
  .custom-input .v-input__slot:after {
    border-color: #ffc0cb;
  }
  
  .custom-btn {
    color: white !important;
  }
  
  .success-btn {
    background-color: #11f1f1 !important;
  }
  
  .error-btn {
    background-color: #ffc0cb !important;
  }
  
  .warning-btn {
    background-color: #f8ffc0 !important;
    color: black !important;
  }
  </style>
  