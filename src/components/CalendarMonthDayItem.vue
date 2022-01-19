<!-- CalendarMonthDayItem.vue -->
<template>
  <li
    class="text-center flex"
    :class="{
      'text-gray-200': !day.isCurrentMonth,
      'rounded-full bg-yellow-100': isToday
    }"
  >
    <div class="grow text-2xl" style="height: 53px; line-height:53px;">{{ label }}</div>
  </li>
</template>
<script>
import dayjs from "dayjs";
export default {
  name: "CalendarMonthDayItem",
  props: {
    day: {
      type: Object,
      required: true
    },
    isCurrentMonth: {
      type: Boolean,
      default: false
    },
    isToday: {
      type: Boolean,
      default: false
    }
  },
  computed: {
    label() {
      return dayjs(this.day.date).format("D");
    }
  }
};
</script>