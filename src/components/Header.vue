<template>
  <div class="header">
    <nav class="navigation">
      <ul>
        <li><router-link to="/">Home</router-link></li>
        <li><router-link to="/contact">Contact</router-link></li>
        <li><router-link to="/about">About</router-link></li>
      </ul>
    </nav>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "Header",
});
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.header {
  padding: 0.825rem;
  background-color: lightgreen;
  .navigation {
    display: inline;
    ul {
      list-style: none;
      li {
        display: inline-block;
      }
      a {
        padding: 0.325rem;
        text-decoration: none;
      }
    }
  }
}
</style>
