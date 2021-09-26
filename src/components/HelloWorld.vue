<template>
  <div>
    <!-- 要给外层div指定合适的宽度 -->
    <div style="width: 600px; margin-top: 16px; margin-left: 16px">
      <baidu-calendar @change="change" :date="date" :range="range" />
    </div>
  </div>
</template>

<script>
import baiduCalendar from "./BaiduCalendar";
export default {
  data() {
    return {
      date: "2021-1-27",
      range: [2015,2025],
    };
  },
  components: {
    baiduCalendar,
  },
  methods: {
    change(obj) {
      console.log("obj", obj);
    },
  },
};
</script>

<style>
</style>