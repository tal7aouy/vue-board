<template>
  <div>
    <apexchart
      width="380"
      type="donut"
      :options="options"
      :series="series"
    ></apexchart>
  </div>
</template>

<script lang="ts" setup>
import { ref } from "vue";
const options = ref({});
const series = ref([44, 55, 41, 17, 15]);
</script>