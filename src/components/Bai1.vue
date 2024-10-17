<script setup lang ="ts">
import {ref, watch} from "vue"
const count = ref(0)
 const handleclick = ()=>{
    count.value++
 };
watch(count, (newValue, oldValue) => {
    alert(`Giá trị của count trước khi bấm: ${oldValue}, Giá trị sau khi đổi của count: ${newValue}`);
});


</script>


<template>
  <button @click="handleclick">Click</button>
</template>



<style>

</style>