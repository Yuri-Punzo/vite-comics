<!-- Descrizione:
Create un nuovo progetto utilizzando Vite e Vue 3 e definite i componenti necessari per strutturare il layout come da screenshot allegato.
Quando la struttura a macroblocchi è pronta, popolate le voci di menu dinamicamente usando i data del componente.
Per oggi diamo priorità alla struttura: quando è tutto bello solido, passiamo al Sass!
Bonus:
Creare un componente aggiuntivo per gestire la fascia azzurra con le icone. -->
<script>
import SiteHeader from './components/SiteHeader.vue'
import SiteMain from "./components/SiteMain.vue"
import SiteFooterTop from "./components/SiteFooterTop.vue"
import SiteFooterCenter from "./components/SiteFooterCenter.vue"
import SiteFooterBottom from "./components/SiteFooterBottom.vue"

export default {
  name: "App",
  components: {
    SiteHeader,
    SiteMain,
    SiteFooterTop,
    SiteFooterCenter,
    SiteFooterBottom
  }
}
</script>

<template>

  <SiteHeader />

  <!-- /site_header -->

  <SiteMain />

  <!-- /site_main -->

  <SiteFooterTop />
  <SiteFooterCenter />
  <SiteFooterBottom />

  <!-- /site_footer -->
</template>

<style lang="scss" scoped>

</style>
