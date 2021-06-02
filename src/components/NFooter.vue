 <template>
  <div class="nFooter">

    <v-list-item
      href="tel:+5493517567466"
    >
      <v-list-item-icon>
        <v-icon>mdi-phone</v-icon>
      </v-list-item-icon>
      <v-list-item-content>
        <v-list-item-title>+54 9 351 756-7466</v-list-item-title>
      </v-list-item-content>
    </v-list-item>
    <v-list-item
      href="mailto:info@azucarorigenes.com.ar"
      class="ma-0"
    >
      <v-list-item-icon>
        <v-icon class="ma-0">mdi-email</v-icon>
      </v-list-item-icon>
      <v-list-item-content>
        <v-list-item-title>info@azucarorigenes.com.ar</v-list-item-title>
      </v-list-item-content>
    </v-list-item>
    <v-list-item href="https://goo.gl/maps/qzJ5JLTwFViRavg9A" :target="$vuetify.breakpoint.sm ? '_blank' : ''">
      <v-list-item-icon>
        <v-icon>mdi-map-marker</v-icon>
      </v-list-item-icon>
      <v-list-item-content>
        <v-list-item-title>Isabel la Católica 994, Córdoba Capital</v-list-item-title>
      </v-list-item-content>
    </v-list-item>
  </div>
</template>

<script>
export default {

}
</script>

<style>

</style>
