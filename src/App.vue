<template>
  <div>
    <todo-list v-bind:todos="todos"></todo-list>
  </div>
</template>

<script>
import TodoList from './components/TodoList'

export default {
  name: 'App',
  components: {
    TodoList
  },
  data () {
    return {
      todos: [
        {
          title: 'Todo 1',
          project: 'Project 1',
          done: false
        },
        {
          title: 'Todo 2',
          project: 'Project 3',
          done: false
        },
        {
          title: 'Todo 3',
          project: 'Project 3',
          done: false
        },
        {
          title: 'Todo 4',
          project: 'Project 4',
          done: true
        }
      ]
    }
  }
}
</script>
