<template>
  <div class="navbar">
    <h1>Booking</h1>
    <div class="navbar__buttons">
      <LogRegButton @click="$router.push('/signup')">Регистрация</LogRegButton>
      <LogRegButton>Вход</LogRegButton>
    </div>
  </div>
</template>

<script>
import LogRegButton from '@/components/UI/MyButton.vue';
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'MyNavbar',
  components: { LogRegButton }
});
</script>

<style scoped lang="scss">
.navbar {
  height: 60px;
  display: flex;
  align-items: center;
  border: 2px solid orange;
  justify-content: space-between;
}

.navbar__buttons {
  display: flex;
  gap: 5px;
  margin-right: 30px;
}
</style>
