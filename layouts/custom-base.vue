<script setup lang="ts">
const props = defineProps({
  layoutClass: String,
});
</script>
<template>
  <div
    :class="{
      'slidev-layout w-full h-full': true,
      [props.layoutClass]: props.layoutClass,
    }"
  >
    <slot />

    <Pagination />
  </div>
</template>
