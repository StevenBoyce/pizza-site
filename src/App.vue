<template>
  <div id="app">
    <Nav />
    <div class="background">
      <img
        class="background-img"
        src="../src/assets/images/pizza-oven.jpg"
        alt=""
      />
      <div class="content">
        <router-view />
      </div>
    </div>
  </div>
</template>

<style lang="less">
body {
  margin: 0;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #000000;
  p {
    color: #fbfaf5;
  }
}

#nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}

.background {
  background-size: 100%;
  overflow: hidden;
  position: relative;
  min-height: 80vh;
  img {
    opacity: 0.7;
    position: absolute;
    left: 0;
    top: 0;
    width: 100%;
    height: auto;
  }
  .content {
    //z-index: 10;

    position: relative;
  }
}
</style>
<script>
import Nav from "./components/Nav";
export default {
  components: { Nav },
};
</script>
