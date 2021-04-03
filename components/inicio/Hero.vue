<template>
  <div class="bg-white dark:bg-gray-800 flex relative z-20 items-center overflow-hidden py-20">
    <div class="container mx-auto px-6 lg:px-16 flex relative py-16">
      <div class="sm:w-2/3 lg:w-2/5 flex flex-col relative z-20">
        <span class="w-20 h-2 bg-gray-800 dark:bg-white mb-12" />
        <h1 class="font-bebas-neue uppercase text-6xl sm:text-8xl font-black flex flex-col leading-none dark:text-white text-gray-800">
          Ofertas
          <span class="text-5xl sm:text-7xl">
            inigualables
          </span>
        </h1>
        <p class="text-sm sm:text-base text-gray-700 dark:text-white">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Veniam consequatur obcaecati dicta quam repellat qui vel voluptatem quidem perspiciatis dignissimos eveniet libero veritatis porro quisquam ipsam, explicabo minus, debitis a.
        </p>
        <div class="flex mt-8">
          <a href="#" class="uppercase py-2 px-4 rounded-lg bg-yellow-500 border-2 border-transparent text-white text-md mr-4 hover:bg-yellow-500">
            Ofertas
          </a>
          <a href="#" class="uppercase py-2 px-4 rounded-lg bg-transparent border-2 border-yellow-500 text-yellow-500 dark:text-white hover:bg-yellow-500 hover:text-white text-md">
            Catálogo
          </a>
        </div>
      </div>
      <div class="hidden sm:block sm:w-1/3 lg:w-3/5 relative">
        <img src="/img/Header1.jpg" class=" lg:max-w-xxl m-auto">
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Hero'
}
</script>

<style lang="scss" scoped>

</style>
