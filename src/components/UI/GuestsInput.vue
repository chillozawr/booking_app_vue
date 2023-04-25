<template>
  <button class="guests_button">
    <slot></slot>
  </button>
</template>

<script>
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'GuestsInput'
});
</script>

<style scoped></style>
