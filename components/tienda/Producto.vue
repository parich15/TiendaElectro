<template>
  <div>
    <img loading="lazy" src="https://via.placeholder.com/520" alt="" class="object-cover w-full h-auto shadow-md max-h-56">
    <div class="mt-2 ">
      <h4 class="text-lg font-bold tracking-tight text-gray-800 ">
        Titulo Producto
      </h4>
      <p class="pb-2 text-base text-gray-400 font-extralight">
        Pequeña descripción del producto
      </p>
      <div class="flex justify-between">
        <p class="font-semibold text-gray-500 ">
          Precio
        </p>
        <span class="text-yellow-400 ">Stock</span>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Producto'
}
</script>

<style lang="scss" scoped>

</style>
