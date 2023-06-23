<template>
  <header>
    <h1>{{ title }}</h1>
  </header>
</template>

<script>
/* eslint-disable vue/multi-word-component-names */

export default {
  name: 'AppHeader', // Renamed the component to "AppHeader"
  props: {
    title: String,
  }
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
