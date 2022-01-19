<!-- CalendarDateIndicator.vue -->
<template>
  <h1 class="absolute text-7xl text-white" style="bottom:67px;">{{ selectedYear }}</h1>
  <h2 class="text-2xl text-center">{{ selectedMonth }}</h2>
</template>

<script>
export default {
  props: {
    selectedDate: {
      type: Object,
      required: true
    }
  },

  computed: {
    selectedYear() {
      return this.selectedDate.format("YYYY");
    },
    selectedMonth() {
      return this.selectedDate.format("MMMM");
    }
  }
};
</script>