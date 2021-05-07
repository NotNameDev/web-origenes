<template>
  <v-container>
    <NHome />
    <NAbout />
    <NProduct />
    <NContact />
    <NFooter />
    <NMedia />
    <NSignature />
  </v-container>

</template>

<script>
import NHome from '../components/NHome'
import NAbout from '../components/NAbout'
import NProduct from '../components/NProduct'
import NContact from '../components/NContact'
import NFooter from '../components/NFooter'
import NMedia from '../components/NMedia'
import NSignature from '../components/NSignature'

export default {
  name: 'MainPage',
  components: {
    NHome,
    NAbout,
    NProduct,
    NContact,
    NFooter,
    NMedia,
    NSignature
  }
}
</script>
