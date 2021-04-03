<template>
  <nav class="fixed top-0 z-50 w-screen shadow bg-gradient-to-r from-blue-500 to-blue-600 dark:bg-gray-800">
    <div class="px-8 mx-auto max-w-7xl">
      <div class="flex items-center justify-between h-16">
        <div class="flex items-center ">
          <a class="flex-shrink-0" href="/">
            <img class="w-8 h-8" src="/icons/rocket.svg" alt="Workflow">
          </a>
          <div class="hidden md:block">
            <div class="flex items-baseline ml-10 space-x-4">
              <nuxt-link class="px-3 py-2 text-sm font-medium text-gray-100 rounded-md hover:text-yellow-300 dark:hover:text-white" to="/">
                Inicio
              </nuxt-link>
              <nuxt-link to="/Catalogo" class="px-3 py-2 text-sm font-medium text-gray-100 rounded-md dark:text-white hover:text-yellow-300 dark:hover:text-white">
                Catálogo
              </nuxt-link>
              <nuxt-link class="px-3 py-2 text-sm font-medium text-gray-100 rounded-md hover:text-yellow-300 dark:hover:text-white" to="/Nosotros">
                Sobre Nosotros
              </nuxt-link>
            </div>
          </div>
        </div>
        <div class="block">
          <div class="flex items-center md:ml-6">
            <div class="relative md:ml-3">
              <div class="relative inline-block text-left">
                <div>
                  <button id="options-menu" type="button" class="flex items-center justify-center w-full px-4 py-2 text-sm font-medium text-yellow-200 transition duration-100 ease-in transform rounded-md dark:text-gray-50 hover:scale-125 dark:hover:bg-gray-500 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-offset-gray-100 focus:ring-gray-500" @click="perfil = !perfil">
                    <svg xmlns="http://www.w3.org/2000/svg" height="21pt" viewBox="0 0 511 511.99913" width="21pt" class="fill-current "><path d="m512.496094 172v80c0 11.046875-8.953125 20-20 20h-13.152344l-8.425781 74.988281c-1.148438 10.21875-9.804688 17.765625-19.851563 17.769531-.746094 0-1.496094-.042968-2.257812-.128906-10.976563-1.230468-18.875-11.132812-17.640625-22.105468l10.421875-92.753907c1.136718-10.117187 9.691406-17.769531 19.875-17.769531h11.035156v-40h-432v40h341c11.046875 0 20 8.957031 20 20 0 11.046875-8.953125 20-20 20h-307.226562l19.75 164.761719c2.40625 20.089843 19.480468 35.238281 39.714843 35.238281h247.125c20.382813 0 37.472657-15.277344 39.75-35.535156 1.230469-10.976563 11.128907-18.871094 22.105469-17.640625 10.976562 1.234375 18.875 11.132812 17.644531 22.109375-4.554687 40.511718-38.730469 71.066406-79.5 71.066406h-247.125c-40.46875 0-74.617187-30.300781-79.433593-70.480469l-20.316407-169.519531h-13.488281c-11.046875 0-20-8.953125-20-20v-80c0-11.046875 8.953125-20 20-20h70.9375l105.683594-143.839844c6.539062-8.898437 19.054687-10.816406 27.957031-4.273437 8.902344 6.539062 10.816406 19.054687 4.277344 27.957031l-88.28125 120.15625h231.589843l-88.285156-120.15625c-6.539062-8.902344-4.625-21.417969 4.277344-27.957031 8.902344-6.542969 21.417969-4.628907 27.960938 4.273437l105.679687 143.839844h70.199219c11.046875 0 20 8.957031 20 20zm-275.996094 160v80c0 11.046875 8.953125 20 20 20 11.042969 0 20-8.953125 20-20v-80c0-11.046875-8.957031-20-20-20-11.046875 0-20 8.953125-20 20zm80 0v80c0 11.046875 8.953125 20 20 20 11.042969 0 20-8.953125 20-20v-80c0-11.046875-8.957031-20-20-20-11.046875 0-20 8.953125-20 20zm-160 0v80c0 11.046875 8.953125 20 20 20 11.042969 0 20-8.953125 20-20v-80c0-11.046875-8.957031-20-20-20-11.046875 0-20 8.953125-20 20zm0 0" /></svg>
                  </button>
                </div>
                <div v-if="perfil" class="absolute right-0 w-56 mt-2 origin-top-right bg-white rounded-md shadow-lg dark:bg-gray-800 ring-1 ring-black ring-opacity-5">
                  <div class="py-1 " role="menu" aria-orientation="vertical" aria-labelledby="options-menu">
                    <a href="#" class="block px-4 py-2 text-gray-700 text-md hover:bg-gray-100 hover:text-gray-900 dark:text-gray-100 dark:hover:text-white dark:hover:bg-gray-600" role="menuitem">
                      <span class="flex flex-col">
                        <span>
                          Ver Carrito
                        </span>
                      </span>
                    </a>
                    <a href="#" class="block px-4 py-2 text-gray-700 text-md hover:bg-gray-100 hover:text-gray-900 dark:text-gray-100 dark:hover:text-white dark:hover:bg-gray-600" role="menuitem">
                      <span class="flex flex-col">
                        <span>
                          Área de Cliente
                        </span>
                      </span>
                    </a>
                    <a href="#" class="block px-4 py-2 text-gray-700 text-md hover:bg-gray-100 hover:text-gray-900 dark:text-gray-100 dark:hover:text-white dark:hover:bg-gray-600" role="menuitem">
                      <span class="flex flex-col">
                        <span>
                          Cerrar Sesión
                        </span>
                      </span>
                    </a>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div class="flex -mr-2 md:hidden">
          <button class="inline-flex items-center justify-center p-2 text-gray-200 rounded-md dark:text-white hover:text-yellow-300 focus:outline-none" @click="abierto = !abierto">
            <svg
              width="20"
              height="20"
              fill="currentColor"
              class="w-8 h-8"
              viewBox="0 0 1792 1792"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path d="M1664 1344v128q0 26-19 45t-45 19h-1408q-26 0-45-19t-19-45v-128q0-26 19-45t45-19h1408q26 0 45 19t19 45zm0-512v128q0 26-19 45t-45 19h-1408q-26 0-45-19t-19-45v-128q0-26 19-45t45-19h1408q26 0 45 19t19 45zm0-512v128q0 26-19 45t-45 19h-1408q-26 0-45-19t-19-45v-128q0-26 19-45t45-19h1408q26 0 45 19t19 45z" />
            </svg>
          </button>
        </div>
      </div>
    </div>
    <div v-if="abierto" class="md:hidden">
      <div class="px-2 pt-2 pb-3 space-y-1 sm:px-3">
        <a class="block px-3 py-2 text-xl font-medium text-center text-gray-100 rounded-md hover:text-yellow-400 dark:hover:text-white" href="/#">
          Inicio
        </a>
        <a class="block px-3 py-2 text-xl font-medium text-center text-gray-100 rounded-md hover:text-yellow-400" href="/#">
          Catálogo
        </a>
        <a class="block px-3 py-2 text-xl font-medium text-center text-gray-100 rounded-md hover:text-yellow-400 dark:hover:text-white" href="/#">
          Sobre Nosotros
        </a>
        <a class="block px-3 py-2 text-xl font-medium text-center text-gray-100 rounded-md hover:text-yellow-400 dark:hover:text-white" href="/#">
          Contacto
        </a>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: 'Navbar',
  data () {
    return {
      perfil: false,
      abierto: false
    }
  }
}
</script>

<style>
.nuxt-link-exact-active{
  color:rgba(252, 211, 77)!important;
}
</style>
