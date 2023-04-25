<template>
  <div class="container"><SearchMain /></div>
</template>

<script>
import SearchMain from '@/components/SearchMain.vue';
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'MainPage',
  components: { SearchMain }
});
</script>

<style scoped lang="scss">
.container {
  //top: 0;
  //bottom: 0;
  //right: 0;
  //left: 0;
  background: rgba(0, 0, 0, 0.5);
  display: flex;
}
</style>
