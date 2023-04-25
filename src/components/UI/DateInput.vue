<template>
  <button class="date_button">
    <slot></slot>
  </button>
</template>

<script>
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'DateInput'
});
</script>

<style scoped></style>
