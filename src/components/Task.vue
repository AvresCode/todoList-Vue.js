<template>
  <div class="task">
    <h3>
      {{ task.text }}
      <i class="fa fa-times"></i>
    </h3>
    <p>{{ task.day }}</p>
  </div>
</template>

<script>
export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: "Task",
  props: {
    task: Object,
  },
};
</script>

<style>
.task {
  background-color: rgb(243, 213, 213);
  margin: 10px;
  padding: 15px;
}

.task h3 {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.task.reminder {
  border-left: 5px solid rgb(118, 186, 118);
}
</style>
