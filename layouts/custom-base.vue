<script setup lang="ts">
const props = defineProps({
  layoutClass: String,
});
</script>
<template>
  <div class="slidev-layout cover {{ props.layoutClass }}">
    <slot />

    <Pagination />
  </div>
</template>
