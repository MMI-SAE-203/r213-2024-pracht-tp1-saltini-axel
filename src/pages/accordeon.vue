<script setup lang="ts">
import { ref } from 'vue'

const maVar = ref(0)
</script>

<template>
<p>Page Accordéon</p> 
  <p>La variable vaut : {{ maVar }}</p>
  <button @click="maVar = maVar === 1 ? 0 : 1">Montrer 1</button>
  <img src="https://image.noelshack.com/fichiers/2020/52/6/1608998191-154387-full.png" v-show="maVar === 1" class="text-2xl"></img>
  <button @click="maVar = maVar === 2 ? 0 : 2">Montrer 2</button>
  <img src="https://www.leparisien.fr/resizer/Spvo6YENyFn9tPG7qwB5xTv0Oe4=/932x582/arc-anglerfish-eu-central-1-prod-leparisien.s3.amazonaws.com/public/GAVNVCNPXXK35KHU2XEPS6XXIM.jpg" v-show="maVar === 2" class="text-2xl"></img>
</template> 
