<template>
  <div class="footer">
    {{ getCopyright }}
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "Footer",

  computed: {
    getCopyright() {
      return `Coded by Yanover - ${new Date().getFullYear()}`;
    },
  },
});
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.footer {
  flex-shrink: 0;
  padding: 1rem;
  color: lightslategrey;
  background-color: lightgray;
  font-style: italic;
}
</style>
