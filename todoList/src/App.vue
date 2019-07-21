<template>
  <div id="app">
    <h2>Jquery To Do List</h2>
    <h4>Simple Todo List with adding and filter bydiff status</h4>
    <input id="inputText"/><button id="addButton">Add</button>
  </div>
</template>

<script>
export default {
  name: 'App'
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
#inputText{
  width: 500px;
  height: 30px;
}
h4{
  font-style: italic;
}
#addButton{
  width: 70px;
  height: 40px;
  color: white;
  background-color: #fc999b;
}
</style>
