<template>
  <main>
    <div class="container">
      <h1>
        欢迎使用 Huang 待办事项！
      </h1>
      <todo-filter />
      <todo-add />
      <todo-list />
    </div>
  </main>
</template>

<script>
import TodoList from "./components/TodoList";
import TodoAdd from "./components/TodoAdd";
import TodoFilter from "./components/TodoFilter.vue";
export default {
  name: "App",
  components: {
    TodoList,
    TodoAdd,
    TodoFilter,
  },
};
</script>

<style>
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
  font-family: Helvetica, "Ping Fang SC", "Microsoft Yahei", sans-serif;
}
main {
  width: 100vw;
  min-height: 100vh;
  display: grid;
  align-items: center;
  justify-items: center;
  background-color: rgb(203, 210, 240);
}
.container {
  width: 60%;
  max-width: 400px;
  box-shadow: 0 0 24px rgba(0, 0, 0, 0.15);
  border-radius: 24px;
  padding: 48px 24px;
  background-color: rgba(245, 246, 252);
}
h1 {
  margin: 24px 0;
  font-size: 28px;
  color: #414873;
}
</style>
