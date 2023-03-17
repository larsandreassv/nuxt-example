<template>
  <div>
    <h1 class="text-xl font-bold text-green-900">Books</h1>
    <span class="flex flex-col" v-for="book in books" v-bind:key="book.id"> {{ book.value }}</span>
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
  {
    id: 5,
    value: "Maze runner",
  },
  {
    id: 6,
    value: "The Matrix",
  },
]);
</script>
