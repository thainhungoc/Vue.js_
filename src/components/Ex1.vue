<script setup lang="ts">
import {ref} from "vue"
let isShow = ref(0)
</script>

<template>
  <div v-if="isShow">Xin chao</div>
  <div v-else-if="isShow == 1">Hello</div>
  <div v-else>Khac</div>
  <br>

  <button @click="() =>{
    isShow = isShow == 0 ? 1 : 0}">Show / Hidden</button>
  <button @click="()=>{
    isShow = 2}">Show other</button>  
</template>

<style scoped lang="scss">

</style>
