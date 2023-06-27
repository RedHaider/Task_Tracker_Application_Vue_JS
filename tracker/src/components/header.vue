<template>
  <header>
    <h1>{{ title }}</h1>
    <Tracker_Button text="Add Task" color="green"/>
  </header>
</template>

<script>
import Tracker_Button from './Tracker_Button';
export default {
  components: { Tracker_Button },
  name: 'AppHeader', // Renamed the component to "AppHeader"
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
</script>

<style scoped>
  header{
    display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 20px;

  }
</style>
