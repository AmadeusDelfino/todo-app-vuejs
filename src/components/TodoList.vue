<template>
  <div>
    <p>Completed tasks: {{todos.filter(todo => {return todo.done === true}).length}}</p>
    <p>Pending tasks: {{todos.filter(todo => {return todo.done === false}).length}}</p>
  </div>
</template>

<script>
export default {
  props: ['todos']
}
</script>
