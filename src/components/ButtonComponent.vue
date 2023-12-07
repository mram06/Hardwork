<template>
  <button>{{ title }}</button>
</template>

<script>
export default {
  name: "ButtonComponent",
  props: {
    title: {
      type: String,
    },
  },
};
</script>

<style lang="scss" scoped>
button {
  color: #fff;

  font-family: "Montserrat", sans-serif;
  font-size: 14px;
  font-weight: 700;
  line-height: 120%;

  height: 40px;
  padding: 10px 24px;

  border-radius: 20px;
  background: #000;
  &:hover {
    background: #2c2c2c;
  }
  &:active {
    background: #181818;
  }
}
</style>
