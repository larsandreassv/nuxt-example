<template>
  <div>
    <h1 class="text-xl text-green-900">Users</h1>
    <p>This is the users page</p>
    <h2 class="text-blue-900">List of users:</h2>
    <span class="flex flex-col text-red-700" v-for="user in users" v-bind:key="user.id"> {{ user.name }} </span>
  </div>
</template>

<script setup lang="ts">
import { ref } from "vue";

const users = ref([
  {
    id: 1,
    name: "Ole",
  },
  {
    id: 1,
    name: "Ole",
  },
  {
    id: 1,
    name: "Eva",
  },
  {
    id: 1,
    name: "Test",
  },
]);
</script>
