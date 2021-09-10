<template>
  <div class="nContact">
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
      color="secondary primary--text"
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
