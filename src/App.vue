<template>
  <div id="app">
    <Header/>
    <Jewelry/>
    <Contact/>
    <Clients/>
    <Footer/>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Footer from './components/Footer.vue'
import Clients from './components/Clients.vue'
import Jewelry from './components/Jewelry.vue'
import Contact from './components/Contact.vue'

export default {
  name: 'App',
  components: {
    Header,
    Footer,
    Clients,
    Jewelry,
    Contact,
  }
}
</script>

<style>
  @import "assets/css/bootstrap.min.css";
  /* @import "assets/css/bootsnav.css"; */
  @import "assets/css/style.css";
  /* @import "assets/css/owl.carousel.min.css"; */
  /* @import "assets/css/owl.theme.default.min.css"; */
  /* @import "assets/css/animate.css"; */
  /* @import "assets/css/responsive.css"; */
  /* @import "assets/css/linearicons.css"; */
  /* @import "assets/css/font-awesome.min.css"; */

</style>
