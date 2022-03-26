<template>
  <div id="nav">
    <router-link to="/" class="routerLink">Home</router-link>
    <font-awesome-icon icon="fa-pizza-slice" @click="routeTo('/')" />
    <router-link to="/about" class="routerLink">About</router-link>
    <font-awesome-icon icon="fa-address-book" @click="routeTo('/about')" />
    <router-link to="/order" class="routerLink">Order Now</router-link>
    <font-awesome-icon icon="fa-store" @click="routeTo('/order')" />
  </div>
</template>

<script>
import router from "../router";

export default {
  name: "Nav",
  methods: {
    routeTo(path) {
      router.push(path);
    },
  },
};
</script>

<style scoped lang="less">
@import "../../src/styles/globals";
#nav {
  color: @primary-color;
  &.router-link-exact-active {
    color: purple;
  }
  a.routerLink {
    color: @primary-color;
    margin: 0 5px 0 15px;
  }
  svg {
    cursor: pointer;
  }
}
</style>
