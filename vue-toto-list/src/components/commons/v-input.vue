<script setup lang="ts">
defineProps({
  type:{
    type:String,
    default: ''
  }
});
</script>

<template>
  <input>
    <slot />
  </input>
</template>
