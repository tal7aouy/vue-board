<template>
  <component :is="layout">
    <router-view />
  </component>
</template>
<script lang="ts" setup>
import { computed } from 'vue'
import { useRouter } from 'vue-router'

const defaultLayout = 'default'

const { currentRoute } = useRouter()

const layout = computed(
  () => `${currentRoute.value.meta.layout || defaultLayout}-layout`
)
</script>

<style>
  @font-face {
  font-family: "Far_Nazanin";
    src: local("Far_Nazanin"), 
    url('./assets/fonts/Far_Nazanin.ttf') format('truetype');
  font-weight: normal;
  font-style: normal;
  };
  * {
    font-family: "Far_Nazanin"
  };
</style>
