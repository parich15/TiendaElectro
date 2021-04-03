<template>
  <div>
    <Navbar />
    <Nuxt />
    <Footer />
  </div>
</template>

<script>
import Footer from '../components/layout/Footer.vue'
import Navbar from '../components/layout/Navbar.vue'
export default {
  components: { Navbar, Footer }

}
</script>
