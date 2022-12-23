<script setup lang="ts">
  import type { PropType } from 'vue'

  type ButtonType = 'button' | 'submit' | 'reset'
  defineProps({
    type: {
      type: String as PropType<ButtonType>,
      required: false,
      default: 'button',
      validator: (value: string) => {
        const _buttonTypes = ['button', 'submit', 'reset']
        return _buttonTypes.includes(value)
      },
    },
  })
</script>

<template>
  <button :type="type">
    <slot></slot>
  </button>
</template>
