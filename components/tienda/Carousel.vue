
<template>
  <div class="relative bg-white shadow-2xl carousel">
    <div class="relative w-full overflow-hidden carousel-inner">
      <!--Slide 1-->
      <input
        id="carousel-1"
        class="carousel-open"
        type="radio"
        name="carousel"
        aria-hidden="true"
        hidden=""
        checked="checked"
      >
      <div class="absolute opacity-0 carousel-item" style="height:100vh;">
        <div class="block w-full h-full text-5xl text-white bg-indigo-500">
          <div class="flex flex-col justify-center h-full px-24 text-left">
            <h1 class="font-semibold md:text-6xl ">
              Producto Destacado
            </h1>
            <h3 class="text-2xl font-light ">
              Breve descripción del producto en cuestión o la oferta la cual se está anunciando.
            </h3>
          </div>
        </div>
      </div>
      <label for="carousel-3" class="absolute inset-y-0 left-0 z-10 hidden w-10 h-10 my-auto ml-2 text-3xl font-bold leading-tight text-center text-black bg-white rounded-full cursor-pointer prev control-1 md:ml-10 hover:text-white hover:bg-blue-700">‹</label>
      <label for="carousel-2" class="absolute inset-y-0 right-0 z-10 hidden w-10 h-10 my-auto mr-2 text-3xl font-bold leading-tight text-center text-black bg-white rounded-full cursor-pointer next control-1 md:mr-10 hover:text-white hover:bg-blue-700">›</label>

      <!--Slide 2-->
      <input
        id="carousel-2"
        class="carousel-open"
        type="radio"
        name="carousel"
        aria-hidden="true"
        hidden=""
      >
      <div class="absolute opacity-0 carousel-item" style="height:100vh;">
        <div class="block w-full h-full text-5xl text-center text-white bg-yellow-500">
          <div class="flex flex-col justify-center h-full px-24 text-left">
            <h1 class="font-semibold md:text-6xl ">
              Producto Destacado
            </h1>
            <h3 class="text-2xl font-light ">
              Breve descripción del producto en cuestión o la oferta la cual se está anunciando.
            </h3>
          </div>
        </div>
      </div>
      <label for="carousel-1" class="absolute inset-y-0 left-0 z-10 hidden w-10 h-10 my-auto ml-2 text-3xl font-bold leading-tight text-center text-black bg-white rounded-full cursor-pointer prev control-2 md:ml-10 hover:text-white hover:bg-blue-700">‹</label>
      <label for="carousel-3" class="absolute inset-y-0 right-0 z-10 hidden w-10 h-10 my-auto mr-2 text-3xl font-bold leading-tight text-center text-black bg-white rounded-full cursor-pointer next control-2 md:mr-10 hover:text-white hover:bg-blue-700">›</label>

      <!--Slide 3-->
      <input
        id="carousel-3"
        class="carousel-open"
        type="radio"
        name="carousel"
        aria-hidden="true"
        hidden=""
      >
      <div class="absolute opacity-0 carousel-item" style="height:100vh;">
        <div class="block w-full h-full text-5xl text-center text-white bg-blue-700">
          <div class="flex flex-col justify-center h-full px-24 text-left">
            <h1 class="font-semibold md:text-6xl ">
              Producto Destacado
            </h1>
            <h3 class="text-2xl font-light ">
              Breve descripción del producto en cuestión o la oferta la cual se está anunciando.
            </h3>
          </div>
        </div>
      </div>
      <label for="carousel-2" class="absolute inset-y-0 left-0 z-10 hidden w-10 h-10 my-auto ml-2 text-3xl font-bold leading-tight text-center text-black bg-white rounded-full cursor-pointer prev control-3 md:ml-10 hover:text-white hover:bg-blue-700">‹</label>
      <label for="carousel-1" class="absolute inset-y-0 right-0 z-10 hidden w-10 h-10 my-auto mr-2 text-3xl font-bold leading-tight text-center text-black bg-white rounded-full cursor-pointer next control-3 md:mr-10 hover:text-white hover:bg-blue-700">›</label>

      <!-- Add additional indicators for each slide-->
      <ol class="carousel-indicators">
        <li class="inline-block mr-3">
          <label for="carousel-1" class="block text-4xl text-white cursor-pointer carousel-bullet hover:text-blue-700">•</label>
        </li>
        <li class="inline-block mr-3">
          <label for="carousel-2" class="block text-4xl text-white cursor-pointer carousel-bullet hover:text-blue-700">•</label>
        </li>
        <li class="inline-block mr-3">
          <label for="carousel-3" class="block text-4xl text-white cursor-pointer carousel-bullet hover:text-blue-700">•</label>
        </li>
      </ol>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Carousel'
}
</script>

<style>
.carousel-open:checked + .carousel-item {
position: static;
opacity: 100;
}
.carousel-item {
    -webkit-transition: opacity 0.6s ease-out;
    transition: opacity 0.6s ease-out;
}
#carousel-1:checked ~ .control-1,
#carousel-2:checked ~ .control-2,
#carousel-3:checked ~ .control-3 {
    display: block;
}
.carousel-indicators {
    list-style: none;
    margin: 0;
    padding: 0;
    position: absolute;
    bottom: 2%;
    left: 0;
    right: 0;
    text-align: center;
    z-index: 10;
}
#carousel-1:checked ~ .control-1 ~ .carousel-indicators li:nth-child(1) .carousel-bullet,
#carousel-2:checked ~ .control-2 ~ .carousel-indicators li:nth-child(2) .carousel-bullet,
#carousel-3:checked ~ .control-3 ~ .carousel-indicators li:nth-child(3) .carousel-bullet {
    color: #2b6cb0;  /*Set to match the Tailwind colour you want the active one to be */
}
</style>
