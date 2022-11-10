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
