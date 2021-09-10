<template>
  <div class="nStars2">
    <div class="stars"></div>
    <div class="twinkling"></div>
    <v-img
      class="logoStars"
      src="../assets/img/origenes_logo_blanco.png"
      contain
      height="150"
    ></v-img>
  </div>
</template>

<script>
export default {

}
</script>

<style>
.nStars2 {
  display: flex;
  justify-content: center;
  align-items: center;
}
/* ==============================================================================================
SED Innovations
https://sed.am
https://mkrtchyan.ga
================================================================================================= */

@keyframes move-twink-back {
    from {background-position:0 0;}
    to {background-position:-10000px 5000px;}
}
@-webkit-keyframes move-twink-back {
    from {background-position:0 0;}
    to {background-position:-10000px 5000px;}
}
@-moz-keyframes move-twink-back {
    from {background-position:0 0;}
    to {background-position:-10000px 5000px;}
}
@-ms-keyframes move-twink-back {
    from {background-position:0 0;}
    to {background-position:-10000px 5000px;}
}

.logoStars {
  z-index: 3;
}

.stars, .twinkling {
  position:absolute;
  top:0;
  left:0;
  right:0;
  bottom:0;
  width:100%;
  height:300px;
  display:block;
  margin:
}

.stars {
  background:#1a586a url('../assets/img/stars.png') repeat top center;
  z-index:0;
}

.twinkling{
  background:transparent url('../assets/img/twinkling3.png') repeat top center;
  z-index:1;

  -moz-animation:move-twink-back 200s linear infinite;
  -ms-animation:move-twink-back 200s linear infinite;
  -o-animation:move-twink-back 200s linear infinite;
  -webkit-animation:move-twink-back 200s linear infinite;
  animation:move-twink-back 200s linear infinite;
}
</style>
