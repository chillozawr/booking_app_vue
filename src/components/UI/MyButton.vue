<template>
  <button class="button">
    <slot></slot>
  </button>
</template>

<script>
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'MyButton'
});
</script>

<style scoped lang="scss">
.button {
  display: block;
  background-color: transparent;
  border: 1px solid blue;
  padding: 5px 10px;
}
</style>
