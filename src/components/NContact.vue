<template>
  <div class="nContact">
    <form name="contact" method="POST" data-netlify="true">
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
      color="accent primary--text"
      elevation="5"
      x-large width="100%"
    >
    Enviar
    </v-btn>
    </form>
  </div>
</template>

<script>
export default {

}
</script>

<style>

</style>
