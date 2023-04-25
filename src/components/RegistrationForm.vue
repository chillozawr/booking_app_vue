<template>
  <div class="wrapper">
    <form class="reg_form" @submit.prevent="log">
      <input type="text" placeholder="Телефон" />
      <input type="text" placeholder="Имя" />
      <input type="text" placeholder="Фамилия" />
      <input type="text" placeholder="Пол" />
      <input type="text" placeholder="Эл. почта" />
      <!--      <button type="submit">Зарегистрироваться</button>-->
      <MyButton type="submit">Зарегистрироваться</MyButton>
    </form>
  </div>
</template>

<script>
import { defineComponent } from 'vue';
import MyButton from '@/components/UI/MyButton.vue';

export default defineComponent({
  name: 'RegistrationForm',
  components: { MyButton },
  methods: {
    log() {
      alert('submit');
    }
  }
});
</script>

<style scoped lang="scss">
.wrapper {
  margin: 0 auto;
  background-color: yellow;
}

.reg_form {
  display: flex;
  flex-direction: column;
  padding: 3rem 4rem;
  gap: 1rem;

  input {
    padding: 0.5rem 1rem;
  }

  button {
    align-self: flex-end;
  }
}
</style>
