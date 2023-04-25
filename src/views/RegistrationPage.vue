<template>
  <div><RegistrationForm /></div>
</template>

<script>
import { defineComponent } from 'vue';
import RegistrationForm from '@/components/RegistrationForm.vue';
export default defineComponent({
  name: 'RegistrationPage',
  components: { RegistrationForm }
});
</script>

<style scoped lang="scss"></style>
