<template>
  <div class="nContact">
    <v-row>
    <v-col cols="12">
      <h1 class="text-center text-uppercase mb-3">Contacto</h1>
      <p></p>
      <p>Por ventas, consultas o más información puede contactarse con nosotros por WhatsApp o completando el siguiente formulario:</p>
      <p></p>
    </v-col>
    </v-row>
    <v-text-field
      label="Nombre"
      outlined
      dense
    ></v-text-field>
    <v-text-field
      label="E-mail"
      outlined
      dense
    ></v-text-field>
    <v-text-field
      label="Asunto"
      outlined
      dense
    ></v-text-field>
    <v-textarea
      outlined
      label="Mensaje"
    ></v-textarea>
    <v-btn
      color="info white--text"
      elevation="5"
      x-large width="100%"
    >
    Enviar
    </v-btn>
  </div>
</template>

<script>
export default {

}
</script>

<style>

</style>
