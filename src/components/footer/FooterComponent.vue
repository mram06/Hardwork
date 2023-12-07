<template>
  <footer class="footer">
    <div class="container">
      <div class="footer__body">
        <div class="footer__row">
          <div class="footer__logo">
            <router-link to="/">HARD<span>WORK</span></router-link>
          </div>
          <div class="footer__info">
            <ul>
              <router-link to="#"><li>Про сервіс</li></router-link>
              <router-link to="#"><li>FAQ</li></router-link>
            </ul>
            <ul>
              <router-link to="#"><li>Умови користування</li></router-link>
              <router-link to="#"><li>Політика приватності</li></router-link>
            </ul>
          </div>
          <div class="footer__socials">
            <router-link to="#"
              ><img src="@/assets/img/icons/facebook.svg"
            /></router-link>
            <router-link to="#"
              ><img src="@/assets/img/icons/linkedin.svg"
            /></router-link>
            <router-link to="#"
              ><img src="@/assets/img/icons/instagram.svg"
            /></router-link>
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "FooterComponent",
};
</script>

<style lang="scss" scoped>
.footer {
  &__body {
    background: #040404;
    vertical-align: middle;

    padding: 32px 123px;
    a {
      color: white;
    }
    li {
      font-size: 14px;
      line-height: 120%;
    }
  }

  &__row {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  &__logo {
    font-family: "Poppins", sans-serif;
    font-size: 37.5px;
    line-height: 120%;
    span {
      font-style: italic;
    }
  }

  &__info {
    display: flex;
    gap: 20px;
    justify-content: space-between;
    width: 392px;
    a:first-child li {
      margin: 0 0 8px 0;
    }
  }

  &__socials {
    display: flex;
    gap: 20px;
  }
}
</style>
