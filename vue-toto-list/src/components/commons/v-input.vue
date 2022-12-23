<script setup lang="ts">
  defineProps({
    type: {
      type: String,
      default: '',
    },
  })
</script>

<template>
  <Input :type="type">
    <slot></slot>
  </Input>
</template>
