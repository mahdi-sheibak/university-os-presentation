<script setup lang="ts">
import CustomBase from "./custom-base.vue";
</script>
<template>
  <CustomBase
    layoutClass="cover bg-no-repeat bg-center bg-cover my-auto grid-content-center"
  >
    <slot />
  </CustomBase>
</template>
