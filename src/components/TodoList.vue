<template>
  <div>
    <div v-for="todo in todos" v-bind:key="todo.id">
      <TodoItem v-bind:todo="todo" />
    </div>
  </div>
</template>
<script>
import TodoItem from "./TodoItem.vue";
export default {
  name: "TodoList",
  components: { TodoItem },
  data() {
    return {
      todos: [
        { id: 1, title: "Todo one", completed: true },
        { id: 2, title: "Todo two", completed: false },
        { id: 3, title: "Todo three", completed: true }
      ]
    };
  }
};
</script>
<style scoped>
</style>