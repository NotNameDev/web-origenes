<template>
  <div class="mainPage">
    <NNavbar />
    <v-container fluid>
      <v-fab-transition>
        <v-btn
          color="#25d366"
          fixed
          fab
          large
          dark
          bottom
          right
          class="mb-5"
          href="https://wa.me/5493516451916"
          target="_blank"
        >
          <v-icon x-large>mdi-whatsapp</v-icon>
        </v-btn>
      </v-fab-transition>
      <div class="d-flex justify-center n-width-complete">
        <v-card
          elevation="0"
        >
          <v-card-text>
            <NHome @click="$vuetify.goTo(this.$refs.contact)" />
            <v-row>
              <v-col cols="12">
                <h1 class="text-center text-uppercase mb-3">Nosotros</h1>
                <!--Falta mejorar el texto-->
                <p>Somos una empresa familiar que se dedica exclusivamente al fraccionado, comercialización y distribución de azúcar. Contamos con más de 10 años de experiencia en el rubro. Nuestras sedes son en Tucumán y Córdoba Capital</p>
              </v-col>
            </v-row>
            <v-row>
              <v-col>
                <NAbout ref="about"/>
              </v-col>
            </v-row>
            <NProduct ref="product"/>
            <v-row>
              <v-col cols="12">
                <h1 class="text-center text-uppercase mb-3">Contacto</h1>
                <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Esse velit doloremque quo beatae quam eum, tempore consectetur, quia blanditiis adipisci earum atque. Alias impedit aspernatur, saepe molestiae omnis ducimus cumque, sit corporis tempore mollitia rem sint esse placeat itaque ea, reiciendis numquam!</p>
              </v-col>
              <v-col
                cols="12"
                lg="6"
                md="6"
                sm="6"
                xs="12"
              >
                <NContact ref="contact"/>
              </v-col>
              <v-col
                class="d-flex flex-column"
                cols="12"
                lg="6"
                md="6"
                sm="6"
                xs="12"
              >
                <NFooter />
                <NMap class="flex-grow-1 elevation-4"/>
              </v-col>
            </v-row>
            <NMedia />
          </v-card-text>
        </v-card>
      </div>
    </v-container>
    <NSignature />
  </div>

</template>

<script>
import NNavbar from '../components/NNavbar'
import NHome from '../components/NHome'
import NAbout from '../components/NAbout'
import NProduct from '../components/NProduct'
import NContact from '../components/NContact'
import NFooter from '../components/NFooter'
import NMedia from '../components/NMedia'
import NSignature from '../components/NSignature'
import NMap from '../components/NMap'

export default {
  name: 'MainPage',
  components: {
    NNavbar,
    NHome,
    NAbout,
    NProduct,
    NContact,
    NFooter,
    NMedia,
    NSignature,
    NMap
  }
}
</script>
