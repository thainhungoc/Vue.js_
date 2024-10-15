<script setup lang="ts">
  let imgUrl="https://i.pinimg.com/control/564x/62/d5/e7/62d5e7673f1ce5043bd266f6dbba99c8.jpg" 
  let test = true

  function testFunc(a:number){
  console.log("da vao", a)
  test = !test
  console.log("gia tri cua test", test)
}
  function enterKey(){
    console.log("enter key")
  }
</script>

<template>
  <img :src="imgUrl" alt="Khong the tai hinh anh">
  <img v-bind:src="imgUrl" alt="">
  <br>
  <h1 :class="test ? 'test' : ''"> Hello</h1>
  <button v-on:click="testFunc(5)">Change Color</button>

  <input @keydown.enter="enterKey" type="text">

</template>

<style scoped lang ="scss">
  .test{
    color: yellow;
    }
</style>
