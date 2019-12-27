<template>
  <div id="app">
    <div class="container">
      <div class="wrapper">
        <Search />
        <TodoList />
        <Add />
      </div>
    </div>
  </div>
</template>

<script>
import Search from "./components/Search.vue";
import TodoList from "./components/TodoList.vue";
import Add from "./components/Add.vue";
export default {
  name: "app",
  components: {
    Search,
    TodoList,
    Add
  }
};
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.wrapper {
  width: 400px;
  height: 400px;
  margin: 0 auto;
}
</style>
