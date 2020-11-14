<template>
  <div class="filters">
    <span v-for="filter in filters" :key="filter.value" class="filter">
      {{ filter.label }}
    </span>
    <span class="filter active">全部</span>
    <span class="filter">已完成</span>
    <span class="filter">未完成</span>
  </div>
</template>

<script>
export default {
  name: "TodoFilter",
  setup() {
    const filters = [
      { label: "全部", value: "all" },
      { label: "已完成", value: "done" },
      { label: "未完成", value: "todo" },
    ];
    return [filters];
  },
};
</script>

<style>
.filters {
  display: flex;
  margin: 24px 2px;
  color: #c0c2ce;
  font-size: 14px;
}
.filters .filter {
  margin-right: 14px;
  transition: 0.8s;
}
.filters .filters.active {
  color: #6b729c;
  transform: scale(1.2);
}
</style>
