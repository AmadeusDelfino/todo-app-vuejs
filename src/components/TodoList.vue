<template>
  <div>
    <todos-overview v-bind:todos="todos"></todos-overview>
    <todo v-for="todo in todos" v-bind:todo="todo" :key="todo.title"></todo>
  </div>
</template>

<script>
import Todo from './Todo'
import TodosOverview from './TodosOverview'

export default {
  props: ['todos'],
  components: {
    Todo,
    TodosOverview
  }
}
</script>
