<template>
  <div class="relative w-full max-w-xl">
    <div>
      <input
        v-model="minprice"
        type="range"
        step="100"
        :min="min"
        :max="max"
        class="absolute z-20 w-full h-2 bg-transparent opacity-0 appearance-none cursor-pointer pointer-events-none"
        @input="mintrigger"
      >

      <input
        v-model="maxprice"
        type="range"
        step="100"
        :min="min"
        :max="max"
        class="absolute z-20 w-full h-2 opacity-0 appearance-none cursor-pointer pointer-events-none"
        @input="maxtrigger"
      >

      <div class="relative z-10 h-2">
        <div class="absolute top-0 left-0 z-30 w-6 h-6 -mt-2 -ml-1 bg-yellow-500 rounded-full" :style="'left: '+minthumb+'%'" />

        <div class="absolute top-0 right-0 z-30 w-6 h-6 -mt-2 -mr-3 bg-yellow-500 rounded-full" :style="'right: '+maxthumb+'%'" />
        <div class="absolute top-0 bottom-0 left-0 right-0 z-10 bg-gray-200 rounded-md" />

        <div class="absolute top-0 bottom-0 z-20 bg-yellow-500 rounded-md" :style="'right:'+maxthumb+'%; left:'+minthumb+'%'" />
      </div>
    </div>

    <div class="flex items-center justify-between py-5">
      <div>
        <input v-model="minprice" type="text" maxlength="5" class="w-24 px-3 py-2 text-center bg-gray-100 rounded focus:ring-1 ring-yellow-100 focus:outline-none " @input="mintrigger">
      </div>
      <div>
        <input v-model="maxprice" type="text" maxlength="5" class="w-24 px-3 py-2 text-center bg-gray-100 rounded focus:ring-1 ring-yellow-100 focus:outline-none" @input="maxtrigger">
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Slider',
  data () {
    return {
      minprice: 20,
      maxprice: 5000,
      min: 100,
      max: 5000,
      minthumb: 0,
      maxthumb: 0
    }
  },
  methods: {
    mintrigger () {
      this.minprice = Math.min(this.minprice, this.maxprice - 500)
      this.minthumb = ((this.minprice - this.min) / (this.max - this.min)) * 100
    },

    maxtrigger () {
      this.maxprice = Math.max(this.maxprice, this.minprice + 500)
      this.maxthumb = 100 - (((this.maxprice - this.min) / (this.max - this.min)) * 100)
    }
  }
}
</script>

<style  scoped>
input[type=range]::-webkit-slider-thumb {
pointer-events: all;
width: 24px;
height: 24px;
-webkit-appearance: none;
/* @apply w-6 h-6 appearance-none pointer-events-auto; */
  }
</style>
