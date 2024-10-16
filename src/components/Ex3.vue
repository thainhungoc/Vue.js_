<script setup lang="ts">
import {ref} from "vue"
let userList = [
    {
        id: 2,
        userName:"Ngoc",
        password:"123",
        gender: false,
    },
    {
        id: 2,
        userName:"Thanh",
        password:"456",
        gender: true
    },
    {
        id: 3,
        userName:"Huy",
        password:"789",
        gender: true
    }
]
</script>

<template>
    <table>
    <thead>
      <tr>
        <th>STT</th>
        <th>userName</th>
        <th>password</th>
        <th>gender</th>
      </tr>
    </thead>
    <tbody>
      <tr v-for="(user, index) in userList" :key="user.id">
        <td>{{ index + 1 }}</td>
        <td>{{ user.userName }}</td>
        <td>{{ user.password }}</td>
        <td>{{ user.gender ? "nam" : "nữ" }}</td>
      </tr>
    </tbody>
  </table>
</template>

<style scoped lang="scss">
      table, th, td, tr {
    border: 1px solid black;
    border-collapse: collapse;
    text-align: center;
  }
</style>
