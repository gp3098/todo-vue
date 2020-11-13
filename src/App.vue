<template>
  <main>
    <div class="container">
      <h1>
        欢迎使用 Huang 待办事项！
      </h1>
      <div class="input-add">
        <input type="text" name="todo" id="todo" />
        <button>
          <i class="plus"></i>
        </button>
      </div>
      <div class="filters">
        <span class="filter active">全部</span>
        <span class="filter">已完成</span>
        <span class="filter">未完成</span>
      </div>
      <div class="todo-list">
        <div class="todo-item">
          <label for="">
            <input type="checkbox" name="" id="" />
            Todo 1
            <span class="check-button"></span>
          </label>
        </div>
        <div class="todo-item">
          <label for="">
            <input type="checkbox" name="" id="" />
            Todo 2
            <span class="check-button"></span>
          </label>
        </div>
      </div>
    </div>
  </main>
</template>

<script>
export default {
  name: "App",
};
</script>

<style>

</style>
