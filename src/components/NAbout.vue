<template>
  <div class="nAbout">
      <v-row>
    <v-col cols="12">
      <h1 class="text-center text-uppercase mb-3">Quiénes Somos</h1>
      <p>Somos Fraccionadora Orígenes, una empresa familiar que se dedica al fraccionado, comercialización y distribución de azúcar común tipo A.</p>
      <p>Contamos con más de 10 años de experiencia en el rubro y clientes que nos eligen desde distintos puntos de Argentina por nuestro compromiso, seriedad y la calidad de nuestros productos.</p>
      <p>Tenemos dos sedes, la principal en Tucumán y otra en Córdoba Capital.</p>
    </v-col>
  </v-row>
  <v-carousel
    :show-arrows="!$vuetify.breakpoint.smAndDown"
    cycle
  >
    <v-carousel-item
      v-for="(item,i) in items"
      :key="i"
      :src="item.src"
    ></v-carousel-item>
  </v-carousel>
  </div>
</template>

<script>
export default {
  data () {
    return {
      items: [
        {
          src: require('../assets/img/Azucar-01.jpeg')
        },
        {
          src: require('../assets/img/Azucar-02.jpeg')
        },
        {
          src: require('../assets/img/Azucar-03.jpeg')
        },
        {
          src: require('../assets/img/Azucar-04.jpeg')
        },
        {
          src: require('../assets/img/Azucar-05.jpeg')
        }
      ]
    }
  }
}
</script>

<style>

</style>
