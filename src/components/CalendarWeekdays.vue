<!-- CalendarWeekdays.vue -->
<template>
  <ol class="grid grid-cols-7">
    <li v-for="weekday in weekdays" :key="weekday" class="text-center bg-zinc-500 text-white">{{ weekday }}</li>
  </ol>
</template>
<script>
const WEEKDAYS = ["Mon", "Tue", "Wed", "Thu", "Fri", "Sat", "Sun"];
export default {
  name: 'CalendarWeekdays',
 
  computed: {
    weekdays() {
      return WEEKDAYS
    }
  }
}
</script>