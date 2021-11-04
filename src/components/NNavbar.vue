<template>
  <div class="nNavbar">
      <v-app-bar
        color="primary"
        dark
        fixed
      >
        <v-toolbar-title
          style="width: 230px;"
        >
          <v-img
            contain
            height="40px"
            max-width="80px"
            src="../assets/origenes_logo_blanco.png"></v-img>
        </v-toolbar-title>
        <v-spacer></v-spacer>
        <v-tabs
          v-if="$vuetify.breakpoint.mdAndUp"
          right
        >
          <v-tab @click="$vuetify.goTo($parent.$refs.about)">Nosotros</v-tab>
          <v-tab @click="$vuetify.goTo($parent.$refs.product)">Producto</v-tab>
          <v-tab @click="$vuetify.goTo($parent.$refs.contact)">Contacto</v-tab>
        </v-tabs>
        <v-app-bar-nav-icon
          v-if="$vuetify.breakpoint.smAndDown"
          @click.stop="drawer = !drawer"
        ></v-app-bar-nav-icon>
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
            <v-list-item>
              <v-list-item-title
                class="primary--text"
                @click="$vuetify.goTo($parent.$refs.about)"
              >
                Nosotros
              </v-list-item-title>
            </v-list-item>

            <v-list-item>
              <v-list-item-title
                class="primary--text"
                @click="$vuetify.goTo($parent.$refs.product)"
              >
                Producto
              </v-list-item-title>
            </v-list-item>

            <v-list-item>
              <v-list-item-title
                class="primary--text"
                @click="$vuetify.goTo($parent.$refs.contact)"
              >
                Contacto
              </v-list-item-title>
            </v-list-item>
          </v-list-item-group>
        </v-list>
      </v-navigation-drawer>
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
