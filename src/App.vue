<script setup>
import { ref } from 'vue'

const count = ref(1)
const increment = () => {
  return ++count.value
}
</script>

<template>
  <section>
    <img alt="Vue logo" class="logo" src="./assets/logo.svg" width="125" height="125" />
    <p>Валуэ: {{ count }}</p>
    <button @click="increment">Добавим + 1 ?</button>
  </section>
</template>

<style scoped lang="scss">
section {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  gap: 20px;
  height: 100vh;
}

button {
  background: hsla(160, 100%, 37%, 1);
  border: none;
  display: flex;
  align-items: center;
  justify-content: center;
  color: #fff;
  border-radius: 100px;
  font-size: 16px;
  max-width: 360px;
  width: 100%;
  height: 56px;
  cursor: pointer;
}
</style>
