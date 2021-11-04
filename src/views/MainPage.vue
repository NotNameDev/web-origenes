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
              <v-col>
                <NAbout ref="about"/>
              </v-col>
            </v-row>
            <NProduct ref="product"/>
            <v-row>
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
