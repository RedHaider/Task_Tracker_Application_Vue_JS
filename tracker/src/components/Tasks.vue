<template>
    <div>
      <div 
       v-for="task in tasks" :key="task.id">
       <task @toggle-reminder="$emit('toggle-reminder',task.id)" @delete-task="$emit('delete-task',task.id)" :task="task" />
      </div>
    </div>
  </template>
  
  <script>
  /* eslint-disable vue/multi-word-component-names */
  import Task from './Task'
  export default {

    name: 'Tasks',
    props: {
      tasks: Array,
    },
    components: {
      Task,
    },
    emits:['delete-task','toggle-reminder'],
  }
  /* eslint-enable vue/multi-word-component-names */
  </script>
  