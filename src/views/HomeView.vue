<template>
  <div class="hero">
    <div class="container">
      <div class="hero__body">
        <h1 class="hero__title">СЕРВІС ДЛЯ ПОШУКУ РОБОТИ В IT</h1>
        <button-component title="Всі вакансії" />
      </div>
    </div>
  </div>
  <div class="subscribe">
    <div class="container">
      <div class="subscribe__body">
        <h2 class="subscribe__title">Підписатися на розсилку</h2>
        <div class="subscribe__input">
          <input type="text" placeholder="Email" />
          <button-component title="Підписатись" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import ButtonComponent from "@/components/ButtonComponent.vue";

export default {
  name: "HomeView",
  components: { ButtonComponent },
};
</script>

<style lang="scss" scoped>
.hero {
  button {
    margin: 40px 0 0 0;
  }
  &__body {
    height: 809px;
    background: url("@/assets/img/background/background.png") top right
      no-repeat;
    padding: 250px 0 0 132px;
  }

  &__title {
  }
}

.subscribe {
  &__body {
    text-align: center;
    background: #e1e1e1;
    padding: 48px 0;
  }

  &__title {
  }

  &__input {
    margin: 0 auto;
    margin-top: 20px;
    max-width: 378px;
    height: 40px;
    border-radius: 20px;
    border: 1px solid #000;
    border-right: none;

    display: flex;
    justify-content: space-between;
    input {
      background: none;
      padding: 10px 0 10px 24px;

      font-size: 14px;
    }
  }
}
.container {
}
</style>
