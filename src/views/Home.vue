<template>
  <div id="app">
    <Todos v-bind:todos="todos" />
  </div>
</template>

<script>
import Todos from '../components/Todos';

export default {
  name: 'Home',
  components: {
    Todos
  },
  data() {
    return {
      todos: [
      {
        id: 1,
        title:'Research what is React',
        completed: false
      },
      {
        id: 2,
        title:'Complete presentation slides',
        completed: false
      },
      {
        id: 3,
        title:'Create a demo',
        completed: false
      },
      {
        id: 4,
        title:'Do the presentation',
        completed: false
      }
      ]
    }
  },
}
</script>

<style>
  * {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
  }

  body {
    font-family: Arial, Helvetica, sans-serif;
    line-height: 1.4;
  }

  .btn {
    display: inline-block;
    border: none;
    background: #555;
    color: #fff;
    padding: 7px 20px;
    cursor: pointer;
  }

  .btn:hover {
    background: #666;
  }
</style>
