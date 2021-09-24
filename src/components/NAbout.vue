<template>
  <div class="nAbout">
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
