<template>
  <div class="home">
    <todo v-for="todo in todos" v-bind:key="todo" v-bind:todo="todo"></todo>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import Todo from "@/components/Todo.vue";

export default defineComponent({
  name: "Home",
  components: {
    Todo,
  },
  data() {
    return {
      todos: [
        {
          description: "Première todo",
          created: "12.10.2021",
          deadline: "12.10.2021",
        },
        {
          description: "Deuxième todo",
          created: "12.10.2021",
          deadline: "12.10.2021",
        },
        {
          description: "Troisième todo",
          created: "12.10.2021",
          deadline: "12.10.2021",
        },
      ],
    };
  },
});
</script>
