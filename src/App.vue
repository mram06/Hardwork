<template>
  <div class="wrapper">
    <header-component />
    <router-view />
  </div>
</template>

<script>
import HeaderComponent from "@/components/header/HeaderComponent.vue";

export default {
  name: "App",
  components: {
    HeaderComponent,
  },
};
</script>

<style lang="scss">
@import url(@/assets/style/index.scss);
</style>
