<script setup lang="ts">
import vButton from "../commons/v-button.vue";
import { ref } from "vue";

const message = ref("hello");
const text = ref("ada");
</script>

<template>
  <vButton :type="submit">Click</vButton>
  {{ message }}
</template>
