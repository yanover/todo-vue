<template>
  <!-- HEADER -->
  <Header></Header>
  <!-- CONTENT -->
  <div class="content">
    <router-view />
  </div>
  <!-- FOOTER -->
  <Footer></Footer>
</template>

<script lang="ts">
import Header from "./components/Header.vue";
import Footer from "./components/Footer.vue";

export default {
  name: "app",
  components: {
    Header,
    Footer,
  },
};
</script>

<style lang="scss">
html,
body {
  width: 100%;
  height: 100%;
}

body {
  padding: 0px;
  margin: 0px;
  overflow-x: hidden;
}

.content {
  flex-grow: 1;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  min-height: 100%;
  display: flex;
  flex-direction: column;
  align-items: stretch;

  a {
    color: #2c3e50;
  }
}
</style>
