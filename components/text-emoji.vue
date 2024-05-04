<script setup lang="ts">
const props = defineProps({
  src: String,
  position: String,
  text: String,
});
</script>
<template>
  <div flex justify-center items-center>
    <div v-if="props.position === 'left'">
      <img :src="props.src" alt="" width="60" height="60" />
    </div>
    <div :class="props.position === 'left' ? 'ml-3' : 'mr-3'">
      <span>{{ props.text }}</span>
    </div>
    <div v-if="props.position === 'right'">
      <img :src="props.src" alt="" width="60" height="60" />
    </div>
  </div>
</template>
