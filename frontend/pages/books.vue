<template>
    <div>
      <span v-for="book in books" v-bind:key="book.id"> {{ book }}</span>
    </div>
  </template>
  
  <script setup lang="ts">
  import { ref } from "vue";
  
  const books = ref([
    {
      id: 1,
      value: "Harry potter and the goblet of fire",
    },
    {
      id: 2,
      value: "Dune",
    },
    {
      id: 3,
      value: "The Very Hungry Caterpillar",
    },
    {
      id: 4,
      value: "Lord of the rings",
    },
  ]);
  </script>
  