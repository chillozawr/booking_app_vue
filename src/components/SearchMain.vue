<template>
  <div class="search_main">
    <div class="search_main__inputs">
      <TextInput placeholder="Куда желаете поехать?.." />
      <DateInput>Дата приезда - Дата отъезда</DateInput>
      <GuestsInput>Количество гостей</GuestsInput>
    </div>
    <MyButton>Искать</MyButton>
  </div>
</template>

<script>
import TextInput from '@/components/UI/TextInput.vue';
import DateInput from '@/components/UI/DateInput.vue';
import GuestsInput from '@/components/UI/GuestsInput.vue';
import MyButton from '@/components/UI/MyButton.vue';
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'SearchMain',
  components: { MyButton, GuestsInput, DateInput, TextInput }
});
</script>

<style scoped>
input {
  padding: 5px 10px;
  display: inline-block;
}

.search_main {
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
  gap: 10px;
}

.search_main__inputs {
  display: flex;
  gap: 10px;
  flex-wrap: wrap;
}
</style>
