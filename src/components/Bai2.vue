<script setup lang = "ts">
// let elementId = "heading";
//   let elementClass = "heading"
const list = {
    id:"heading",
    class:"heading"
}
</script>


<template >
  <div id = "app" data-v-app>
    <h1 v-bind="list">Heading</h1>

  </div>
</template>

<style>

</style>