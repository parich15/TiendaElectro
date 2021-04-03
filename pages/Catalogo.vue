<template>
  <div>
    <carousel />
    <div class="py-20 bg-white section ">
      <div class="container flex mx-auto ">
        <div class="w-1/3">
          <div class="flex flex-col p-6 mx-10 rounded shadow-md bg-gray-50 ">
            <div>
              <h2 class="text-2xl font-semibold leading-3 tracking-tight text-yellow-500 ">
                Encuentra lo que necesitas
              </h2>
            </div>
            <div class="pt-10">
              <h4 class="mb-4 text-lg font-bold text-gray-700">
                Categorias
              </h4>
              <select id="" name="Categoría" class="w-2/3 h-8 font-semibold text-gray-600 bg-gray-100 rounded ring-yellow-200 focus:ring-2">
                <option value="Todos">
                  Mostrar Todos
                </option>
                <option value="Electronica">
                  Electrónica
                </option>
                <option value="Electrodomesticos">
                  Electrodomesticos
                </option>
              </select>
            </div>
            <div class="pt-6">
              <h4 class="mb-4 text-lg font-bold text-gray-700">
                Marca
              </h4>
              <select id="" name="Categoría" class="w-2/3 h-8 font-semibold text-gray-600 bg-gray-100 rounded ring-yellow-200 focus:ring-2">
                <option value="Todos">
                  Mostrar Todos
                </option>
                <option value="Electronica">
                  Braun
                </option>
                <option value="Electrodomesticos">
                  Bosch
                </option>
                <option value="Electrodomesticos">
                  ByD
                </option>
                <option value="Electrodomesticos">
                  Samsung
                </option>
              </select>
            </div>
            <div class="py-6">
              <h4 class="mb-4 text-lg font-bold text-gray-700">
                Precio
              </h4>
              <slider />
            </div>
            <div>
              <h4 class="mb-4 text-lg font-bold text-gray-700">
                Filtros Avanzados
              </h4>
              <div class="flex items-center justify-between">
                <div>
                  <input id="Oferta" type="checkbox" name="Oferta">
                  <label for="Oferta"> En Oferta</label>
                </div><div>
                  <input id="Exclusivo" type="checkbox" name="Exclusivo">
                  <label for="Exclusivo"> Exclusivo</label>
                </div><div>
                  <input id="Stock" type="checkbox" name="Stock">
                  <label for="Stock">Sin Stock</label>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div class="w-2/3">
          <div class="grid grid-cols-3 grid-rows-3 gap-y-20">
            <div v-for="i in productos" :key="i" class="flex justify-center w-2/3 mx-auto ">
              <producto />
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Carousel from '../components/tienda/Carousel.vue'
import Producto from '../components/tienda/Producto.vue'
import Slider from '../components/tienda/Slider.vue'

export default {
  name: 'Catalogo',
  components: { Carousel, Producto, Slider },
  data () {
    return {
      productos: 7
    }
  }
}
</script>

<style lang="scss" scoped>

</style>
