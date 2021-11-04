<template>
  <div class="nHome">
    <div class="">
      <v-row justify="end" align="end" class="pa-0 ma-0">
        <v-col
          cols="12"
          class="pa-0 ma-0"
        >
          <v-img
            src="../assets/img/Azucar-05.jpeg"
            cover
            max-height="700"
          ></v-img>
        </v-col>
        <v-col
          cols="8"
          sm="8"
          xs="7"
          class="image-text"
        >
          <p
            class="font-weight-bold white--text d-flex text-end mr-10"
            :class="$vuetify.breakpoint.xs ? '' : 'text-h2'"
          >Lorem ipsum dolor sit amet consectetur, adipisicing elit.</p>
        </v-col>
      </v-row>
    </div>
  </div>
</template>
<script>
export default {
  name: 'NHome'
}
</script>

<style scoped>
  .image-text {
    position: absolute;
  }
</style>
