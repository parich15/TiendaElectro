<template>
  <div class=" flex flex-col lg:flex-row-reverse py-20">
    <div class=" w-5/12">
      <div class=" pl-7">
        <h3 class=" text-4xl leading-8 font-extrabold text-gray-600 dark:text-white tracking-wide sm:leading-9">
          Lo mejor en
          <span class=" text-5xl text-blue-600">
            Electrónica
          </span>
        </h3>
      </div>
      <div class=" pl-7 mt-10">
        <h3 class=" font-semibold text-lg text-gray-700 mb-2 animate-pulse ">
          Semana sin Iva - Del 25 al 30 de Abril
        </h3>
        <p class=" font-normal text-lg text-gray-700">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Ea, aliquid porro ab, reprehenderit tempore odio fugiat tempora obcaecati repudiandae molestiae quia repellat voluptate! Quibusdam provident atque in ea nulla. Iusto
        </p>
      </div>
    </div>
    <div class=" w-7/12">
      <div class="flex flex-wrap items-center justify-center">
        <div class="flex-shrink-0 mx-2 -mb-6 relative overflow-hidden bg-blue-500 rounded-lg max-w-xs shadow-lg">
          <svg class="absolute bottom-0 left-0 mb-8" viewBox="0 0 375 283" fill="none">
            <rect
              x="159.52"
              y="175"
              width="152"
              height="152"
              rx="8"
              transform="rotate(-45 159.52 175)"
              fill="#4696f6"
            />
            <rect
              y="107.48"
              width="152"
              height="152"
              rx="8"
              transform="rotate(-45 0 107.48)"
              fill="#4696f6"
            />
          </svg>
          <div class="relative pt-10 px-10 flex items-center justify-center">
            <div class="block absolute w-48 h-48 bottom-0 left-0 -mb-24 ml-3" />
            <picture>
              <source srcSet="/images/object/5.webp" type="image/webp">
              <source srcSet="/images/object/5.png">
              <img class="relative w-40" src="/images/object/5.png" alt="shopping item">
            </picture>
          </div>
          <div class="relative text-white px-6 pb-6 mt-6">
            <span class="block opacity-75 -mb-1">
              Bosch
            </span>
            <div class="flex justify-between">
              <span class="block font-semibold text-xl">
                Lavadora<br> Xtreme
              </span>
              <span class="bg-white rounded-full text-yellow-500 text-xs font-bold px-3 py-2 leading-none flex items-center">
                150.00€
              </span>
            </div>
          </div>
        </div>
        <div class="flex-shrink-0 mx-2 mb-6 sm:mb-0 relative overflow-hidden bg-yellow-500 rounded-lg max-w-xs shadow-lg">
          <svg class="absolute bottom-0 left-0 mb-8" viewBox="0 0 375 283" fill="none">
            <rect
              x="159.52"
              y="175"
              width="152"
              height="152"
              rx="8"
              transform="rotate(-45 159.52 175)"
              fill="#f3c06b"
            />
            <rect
              y="107.48"
              width="152"
              height="152"
              rx="8"
              transform="rotate(-45 0 107.48)"
              fill="#f3c06b"
            />
          </svg>
          <div class="relative pt-10 px-10 flex items-center justify-center">
            <div class="block absolute w-48 h-48 bottom-0 left-0 -mb-24 ml-3" />
            <img class="relative w-40" src="/images/object/6.png" alt="shopping">
          </div>
          <div class="relative text-white px-6 pb-6 mt-6">
            <span class="block opacity-75 -mb-1">
              Phillips
            </span>
            <div class="flex justify-between">
              <span class="block font-semibold text-xl">
                Lavavajillas
                <br>
                Gx-500
              </span>
              <span class="bg-white rounded-full text-blue-500 text-xs font-bold px-3 py-2 leading-none flex items-center">
                300.00€
              </span>
            </div>
          </div>
        </div>
        <div class="flex-shrink-0 mx-2 mb-6 relative overflow-hidden bg-purple-500 rounded-lg max-w-xs shadow-lg">
          <svg class="absolute bottom-0 left-0 mb-8" viewBox="0 0 375 283" fill="none">
            <rect
              x="159.52"
              y="175"
              width="152"
              height="152"
              rx="8"
              transform="rotate(-45 159.52 175)"
              fill="#a17cf3"
            />
            <rect
              y="107.48"
              width="152"
              height="152"
              rx="8"
              transform="rotate(-45 0 107.48)"
              fill="#a17cf3"
            />
          </svg>
          <div class="relative pt-10 px-10 flex items-center justify-center">
            <div class="block absolute w-48 h-48 bottom-0 left-0 -mb-24 ml-3" />
            <img class="relative w-40" src="/images/object/7.png" alt="shopping">
          </div>
          <div class="relative text-white px-6 pb-6 mt-6">
            <span class="block opacity-75 -mb-1">
              B&D
            </span>
            <div class="flex justify-between">
              <span class="block font-semibold text-xl">
                Taladro<br>Ultra300
              </span>
              <span class="bg-white rounded-full text-purple-500 text-xs font-bold px-3 py-2 leading-none flex items-center">
                70.00€
              </span>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Electronica'
}
</script>

<style lang="scss" scoped>

</style>
