<template>
  <div>
    <hero />
    <presentacion />
    <electrodomesticos />
    <electronica />
    <catalogo-cta />
    <newsletter />
  </div>
</template>

<script>
import CatalogoCta from '../components/inicio/CatalogoCta.vue'
import Electrodomesticos from '../components/inicio/Electrodomesticos.vue'
import Electronica from '../components/inicio/Electronica.vue'
import Hero from '../components/inicio/Hero.vue'
import Newsletter from '../components/inicio/Newsletter.vue'
import Presentacion from '../components/inicio/Presentacion.vue'
export default {
  name: 'Inicio',
  components: { Hero, Presentacion, Electrodomesticos, Electronica, CatalogoCta, Newsletter }
}
</script>

<style>

</style>
