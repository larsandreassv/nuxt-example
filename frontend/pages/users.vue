<template>
  <div>
    <h1 class="text-green">Users</h1>
    <p>This is the users page</p>
    <span class="flex flex-col" v-for="user in users" v-bind:key="user.id"> {{ user.name }} </span>
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
    name: "Adam",
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
