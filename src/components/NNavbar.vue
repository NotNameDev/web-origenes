<template>
  <div class="nNavbar">
    <!-- <v-card
      class="mx-auto overflow-hidden"
    > -->
      <!-- <v-system-bar color="deep-purple darken-3"></v-system-bar> -->

      <v-app-bar
        color="deep-purple accent-4"
        dark
      >
        <v-toolbar-title style="width: 230px; border: solid 2px red;">Azucarera Orígenes</v-toolbar-title>
        <v-spacer></v-spacer>
        <v-tabs
          v-if="$vuetify.breakpoint.mdAndUp"
          right
        >
          <v-tab>Nosotros</v-tab>
          <v-tab>Producto</v-tab>
          <v-tab>Contacto</v-tab>
        </v-tabs>
        <v-app-bar-nav-icon
          v-if="$vuetify.breakpoint.smAndDown"
          @click.stop="drawer = !drawer"
        ></v-app-bar-nav-icon>
      <!-- <template v-slot:extension>
        <v-tabs align-with-title>
          <v-tab>Tab 1</v-tab>
          <v-tab>Tab 2</v-tab>
          <v-tab>Tab 3</v-tab>
        </v-tabs>
      </template> -->
      </v-app-bar>
      <v-navigation-drawer
        v-model="drawer"
        absolute
        right
        temporary
        color="primary--text"
      >
        <v-list
          nav
          dense
        >
          <v-list-item-group
            class="primary--text"
            v-model="group"
            active-class="primary--text text--darken-3"
          >
            <!-- <v-list-item> -->
              <!-- <v-list-item-title class="d-flex justify-end"> -->
                <div class="d-flex justify-end">
                  <v-btn
                    text
                    fab
                    small
                    color="primary"
                    @click="drawer = !drawer"
                  >
                    <v-icon>mdi-close</v-icon>
                  </v-btn>

                </div>
              <!-- </v-list-item-title> -->
            <!-- </v-list-item> -->

            <v-list-item>
              <v-list-item-title class="primary--text">Nosotros</v-list-item-title>
            </v-list-item>

            <v-list-item>
              <v-list-item-title class="primary--text">Producto</v-list-item-title>
            </v-list-item>

            <v-list-item>
              <v-list-item-title class="primary--text">Contacto</v-list-item-title>
            </v-list-item>
          </v-list-item-group>
        </v-list>
      </v-navigation-drawer>

      <v-card-text>
        The navigation drawer will appear from the bottom on smaller size screens.
      </v-card-text>
    <!-- </v-card> -->
  </div>
</template>

<script>
export default {
  name: 'NNavbar',
  data () {
    return {
      drawer: false,
      group: null
    }
  },

  watch: {
    group () {
      this.drawer = false
    }
  }
}
</script>

<style>

</style>
