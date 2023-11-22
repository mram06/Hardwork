<template>
  <header class="header">
    <div class="container">
      <div class="header__body">
        <div class="header__row">
          <div class="header__logo">
            <router-link to="/">HARD<span>WORK</span></router-link>
          </div>
          <nav class="header__menu">
            <ul>
              <router-link to="/about"><li>Вакансії</li></router-link>
              <router-link to="/about"><li>Компанія</li></router-link>
              <router-link to="/about"><li>Аналітика</li></router-link>
              <router-link to="/about"><li>Медіа</li></router-link>
            </ul>
          </nav>
          <div class="header__tools">
            <div class="header__tools-search">
              <img src="@/assets/img/icons/search.svg" />
            </div>
            <div class="header__tools-login">
              <router-link to="#">Увійти</router-link>
            </div>
            <button-component title="Реєстрація" />
          </div>
        </div>
      </div>
    </div>
  </header>
</template>

<script>
import ButtonComponent from "@/components/ButtonComponent.vue";

export default {
  name: "HeaderComponent",
  components: {
    ButtonComponent,
  },
};
</script>

<style lang="scss" scoped>
.header {
  &__body {
    padding: 12px 123px;

    font-family: "Montserrat", sans-serif;
    font-size: 14px;
    font-weight: 700;
    line-height: 120%;
    vertical-align: middle;
  }

  &__row {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  &__logo {
    font-family: "Poppins", sans-serif;
    font-size: 20px;
    span {
      font-style: italic;
    }
  }

  &__menu {
    ul {
      display: flex;
      align-items: center;
      gap: 24px;
    }
  }

  &__tools {
    display: flex;
    align-items: center;
    gap: 24px;
    &-search {
      cursor: pointer;
    }
  }
}
</style>
