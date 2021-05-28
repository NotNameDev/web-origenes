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
          src: require('../assets/img/Origenes_azucar_Page_05.png')
        },
        {
          src: require('../assets/img/Origenes_azucar_Page_06.png')
        },
        {
          src: require('../assets/img/Origenes_azucar_Page_07.png')
        },
        {
          src: require('../assets/img/Origenes_azucar_Page_08.png')
        },
        {
          src: require('../assets/img/Origenes_azucar_Page_09.png')
        },
        {
          src: require('../assets/img/Origenes_azucar_Page_10.png')
        }
      ]
    }
  }
}
</script>

<style>

</style>
