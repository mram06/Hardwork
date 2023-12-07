<template>
  <div class="wrapper">
    <header-component />

    <main class="content">
      <router-view />
    </main>

    <footer-component />
  </div>
</template>

<script>
import HeaderComponent from "@/components/header/HeaderComponent.vue";
import FooterComponent from "@/components/footer/FooterComponent.vue";

export default {
  name: "App",
  components: {
    HeaderComponent,
    FooterComponent,
  },
};
</script>

<style lang="scss">
@import url(@/assets/style/index.scss);
</style>
