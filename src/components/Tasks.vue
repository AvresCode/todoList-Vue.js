<template>
  <div v-for="task in tasks" :key="task.id">
    <!-- <h3>{{ task.text }}</h3> -->
    <Task :task="task" />
  </div>
</template>

<script>
import Task from "./Task";
export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: "Tasks",
  props: {
    tasks: Array,
  },
  components: {
    Task,
  },
};
</script>
