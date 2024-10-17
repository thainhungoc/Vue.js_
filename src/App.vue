<!-- <script setup lang="ts">
import ComB from './ComB.vue';

let count = 5;

let userList = [
  {id: 1, name: "Nhu"},
  {id: 2, name: "Ngoc"}
]

</script>

<template>
  <h1>Component Cha</h1>
  <ComB :count="5" :test="1000" :userList="userList"></ComB>
</template>

<style scoped>

</style> -->

<script setup lang ="ts">
import { ref } from 'vue';
import ComTest from './ComTest.vue';

let slotName = ref('slotC')

function changeSlot() {
  console.log("đã vào")
  if (slotName.value == 'slotC') {
    slotName.value = 'slotB';
  } else {
    slotName.value = 'slotC';
  }
}
</script>

<template>
  <h1>Ccomponent App</h1>
  <ComTest>
    <template #A ={text}>
        <div>
            <button>Click me A</button>
        </div>
    </template>

    <template #B>
        <div>
            <button @click="changeSlot">Click me B</button>
        </div>
    </template>
  </ComTest>
</template>


<style scoped>
</style>

