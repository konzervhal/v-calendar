<template>
  <VCalendar
    :initial-page="{ month: 1, year: 2018 }"
    :attributes="attributes"
  />
</template>

<script setup>
import { ref } from 'vue';

const attributes = ref([
  {
    dot: true,
    dates: [
      new Date(2018, 0, 1), // Jan 1st
      new Date(2018, 0, 10), // Jan 10th
      new Date(2018, 0, 22), // Jan 22nd
    ],
  },
  {
    dot: 'red',
    dates: [
      new Date(2018, 0, 4), // Jan 4th
      new Date(2018, 0, 10), // Jan 10th
      new Date(2018, 0, 15), // Jan 15th
    ],
  },
  {
    dot: {
      style: {
        backgroundColor: 'brown',
      },
    },
    dates: [
      new Date(2018, 0, 12), // Jan 12th
      new Date(2018, 0, 26), // Jan 26th
      new Date(2018, 0, 15), // Jan 15th
    ],
  },
]);
</script>
