<script setup lang="ts">
import { PropType } from 'vue';

interface User{
    id: number,
    name: string
}
defineProps({
    count:{
        type: Number,
        required: true
    }, 
    test:{
        type: Number,
        default: 10
    },
    userList:{
        type: Array as PropType<User[]>,
        required: true
    }

})
</script>

<template>
  <h1>Day la Component B</h1>
  <h2>Gia tri count: {{ count }}</h2>
  <h2>Gia tri test: {{ test }}</h2>
  <li v-for="user in userList " :key="user.id" >{{ user.name }}</li>
</template>

<style scoped>

</style>
