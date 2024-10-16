<script setup lang = "ts">

const isActive = false
const backgroundColor = "blue"
</script>


<template >
    <div v-bind="isActice ? active : notActive" :style="{background:backgroundColor}">block</div>
</template>

<style scoped lang ="scss">
 active{
    background-color: blue;
    color:#fff;
    height: 100px;
    width: 500px;

 }
 notActice{
    background-color: blue;
    color:#0a0a0a;
    height: 100px;
    width: 500px;
 }
</style>