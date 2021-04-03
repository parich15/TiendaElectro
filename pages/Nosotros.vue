<template>
  <div>
    <div class="cabecera clear-filter" filter-color="black">
      <parallax
        class="imagen-cabecera"
        style="background-image:url('/img/sobrenosotros.jpg')"
      />
      <div class="container-cabecera">
        <div class="content-center">
          <h1 class="text-6xl font-semibold leading-6 tracking-wider">
            Sobre Nosotros
          </h1>
        </div>
      </div>
    </div>

    <div class="px-4 py-20 bg-lightblue">
      <div class="flex flex-col max-w-6xl mx-auto md:flex-row">
        <h2 class="w-full mr-8 text-3xl font-extrabold leading-9 text-yellow-500 md:w-1/3">
          Calidad como <span class="text-blue-500">compromiso</span>
        </h2>
        <dl class="w-full md:w-2/3">
          <dt class="mb-4">
            <h3 class="text-xl font-semibold">
              Sobre Tienda Electrónica, quienes somos y dónde estamos?
            </h3>
          </dt>
          <dd class="mb-16">
            <p>
              Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quis excepturi vel laudantium libero et commodi modi soluta aperiam dolorum, laborum eos veniam maxime? In repellat, doloremque nisi vero unde harum.
            </p>
          </dd>
          <dt class="mb-4">
            <h3 class="text-xl font-semibold">
              Nuestros valores y fundamentos
            </h3>
          </dt>
          <dd class="mb-16">
            <p>
              Lorem ipsum dolor sit amet, consectetur adipisicing elit. Assumenda autem repellendus nostrum numquam, ab nemo qui voluptates hic iste labore quisquam consequuntur earum ratione, aliquid id quam vero fuga ducimus.
            </p>
          </dd>
          <dt class="mb-4">
            <h3 class="text-xl font-semibold">
              Evolutivos por naturaleza
            </h3>
          </dt>
          <dd class="mb-16">
            <p>
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptatibus odit sit consequatur obcaecati vero dolorum quos recusandae distinctio placeat. Modi provident at magnam officia eum, minus perferendis corrupti asperiores voluptatem.
            </p>
          </dd>
        </dl>
      </div>
    </div>

    <div class="relative z-20 w-full p-8 bg-white rounded-lg shadow dark:bg-gray-800">
      <p class="text-3xl font-bold text-center text-gray-800 dark:text-white">
        Team Tienda Electrónica
      </p>
      <p class="mb-12 text-xl font-normal text-center text-gray-500 dark:text-gray-200">
        Conoce a nuestro equipo
      </p>
      <div class="flex flex-col items-center w-full md:flex-row justify-evenly">
        <div class="p-4">
          <div class="mb-4 text-center opacity-90">
            <a href="#" class="relative block">
              <img alt="profil" src="https://via.placeholder.com/150" class="object-cover w-40 h-40 mx-auto rounded-full ">
            </a>
          </div>
          <div class="text-center">
            <p class="text-2xl text-gray-800 dark:text-white">
              Daniel Sevilla
            </p>
            <p class="text-xl font-light text-gray-500 dark:text-gray-200">
              CEO
            </p>
            <p class="max-w-xs py-4 font-light text-gray-500 text-md dark:text-gray-400">
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Fugit nemo velit quia ducimus ut, reprehenderit provident alias eum iste sequi neque corporis blanditiis praesentium vel facilis, eius similique. Odit, ullam.
            </p>
          </div>
        </div>
        <div class="p-4">
          <div class="mb-4 text-center opacity-90">
            <a href="#" class="relative block">
              <img alt="fotoperfil" src="https://via.placeholder.com/200" class="object-cover w-40 h-40 mx-auto rounded-full ">
            </a>
          </div>
          <div class="text-center">
            <p class="text-2xl text-gray-800 dark:text-white">
              Paula Caparrós
            </p>
            <p class="text-xl font-light text-gray-500 dark:text-gray-200">
              Marketing Digital
            </p>
            <p class="max-w-xs py-4 font-light text-gray-500 text-md dark:text-gray-400">
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Fugit nemo velit quia ducimus ut, reprehenderit provident alias eum iste sequi neque corporis blanditiis praesentium vel facilis, eius similique. Odit, ullam.
            </p>
          </div>
        </div>
        <div class="p-4">
          <div class="mb-4 text-center opacity-90">
            <a href="#" class="relative block">
              <img alt="profil" src="https://via.placeholder.com/150" class="object-cover w-40 h-40 mx-auto rounded-full ">
            </a>
          </div>
          <div class="text-center">
            <p class="text-2xl text-gray-800 dark:text-white">
              Alex Wisconsin
            </p>
            <p class="text-xl font-light text-gray-500 dark:text-gray-200">
              Especialista Ventas
            </p>
            <p class="max-w-xs py-4 font-light text-gray-500 text-md dark:text-gray-400">
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Fugit nemo velit quia ducimus ut, reprehenderit provident alias eum iste sequi neque corporis blanditiis praesentium vel facilis, eius similique. Odit, ullam.
            </p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Parallax from '../components/Parallax'
export default {
  name: 'Nosotros',
  components: { Parallax }
}
</script>

<style scoped>
.cabecera {
min-height: 100vh;
max-height: 999px;
padding: 0;
color: white;
position: relative;
overflow: hidden;
}
 .cabecera > .content {
margin-top: 12%;
text-align: center;
margin-bottom: 50px;
}
 .cabecera.cabecera-pequeña {
min-height: 60vh;
max-height: 440px;
}
 .cabecera:before {
background-color: rgba(0, 0, 0, .3);
}
 .cabecera > .b-container-cabecera {
z-index: 2;
padding-top: 12vh;
padding-bottom: 40px;
}
 .cabecera .imagen-cabecera {
position: absolute;
background-size: cover;
background-position: center center;
width: 100%;
height: 100%;
z-index: -1;
}
 .cabecera .content-center {
position: absolute;
top: 50%;
left: 50%;
z-index: 2;
-ms-transform: translate(-50%, -50%);
-webkit-transform: translate(-50%, -50%);
transform: translate(-50%, -50%);
text-align: center;
color: #fff;
padding: 0 15px;
width: 100%;
max-width: 880px;
}
 .cabecera .container {
height: 100%;
z-index: 1;
text-align: center;
position: relative;
}
 .cabecera:after, .cabecera:before {
position: absolute;
z-index: 0;
width: 100%;
height: 100%;
display: block;
left: 0;
top: 0;
content: "";
}
 .clear-filter:after, .clear-filter:before {
display: none;
}
.clear-filter[filter-color="black"] {
background: rgba(29, 92, 211, 0.2);
/* For browsers that do not support gradients */
background: -webkit-linear-gradient(90deg, rgba(29, 92, 211, 0.2), rgba(43, 57, 180, 0.7));
/* For Safari 5.1 to 6.0 */
background: -o-linear-gradient(90deg, rgba(29, 92, 211, 0.2), rgba(43, 57, 180, 0.7));
/* For Opera 11.1 to 12.0 */
background: -moz-linear-gradient(90deg, rgba(29, 92, 211, 0.2), rgba(43, 57, 180, 0.7));
/* For Firefox 3.6 to 15 */
background: linear-gradient(0deg, rgba(29, 92, 211, 0.2), rgba(43, 57, 180, 0.7));
/* Standard syntax */
}

</style>
