<template>
  <div id="app">
    <todo-app-component></todo-app-component>
  </div>
</template>

<script>
import todoAppComponent from './components/TodoComponent';

export default {
  name: 'app',
  components: {
    todoAppComponent
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
