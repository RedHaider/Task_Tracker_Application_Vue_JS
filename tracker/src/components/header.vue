<template>
  <header>
    <h1>{{ title }}</h1>
    <Tracker_Button 
    @toggle-add-task="$emit('toggle-add-task')" 
    text="Add Task" 
    color="green"/>
  </header>
</template>

<script>
/* eslint-disable vue/multi-word-component-names */
import Tracker_Button from './Tracker_Button';
export default {
  components: { Tracker_Button },
  name: 'Header', // Renamed the component to "AppHeader"
  props: {
    title:{
      type: String,
      default: 'Hello World',
    },
  components:{
    Tracker_Button,
  }
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
