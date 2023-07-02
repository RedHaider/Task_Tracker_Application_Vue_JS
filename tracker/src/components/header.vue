<template>
  <header>
    <h1>{{ title }}</h1>
    <Tracker_Button 
    @btn-click="$emit('toggle-add-task')"
      :text="showAddTask ? 'Close' : 'Add Task'"
      :color="showAddTask ? 'red' : 'green'"/>
  </header>
</template>

<script>
/* eslint-disable vue/multi-word-component-names */
import Tracker_Button from './Tracker_Button';
export default {
  components: { Tracker_Button },
  name: 'Header', // Renamed the component to "AppHeader"
  props: {
      title: String,
      showAddTask: Boolean,
    },

  }
/* eslint-enable vue/multi-word-component-names */
</script>

<style scoped>
  header{
    display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 20px;

  }
</style>
