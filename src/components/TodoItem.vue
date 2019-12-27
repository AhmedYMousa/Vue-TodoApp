<template>
  <div>
    <input class="checkbox" type="checkbox" v-bind:checked="todo.completed" v-bind:disabled="true" />
    <label>{{todo.title}}</label>
  </div>
</template>
<script>
export default {
  name: "TodoItem",
  props: ["todo"]
};
</script>
<style scoped>
</style>