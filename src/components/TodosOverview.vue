<template>
    <div>
      <p>Completed tasks: {{completeds.length}}</p>
      <p>Pending tasks: {{pendings.length}}</p>
    </div>
</template>

<script>
export default {
  props: ['todos'],
  computed: {
    completeds: function () {
      return this.todos.filter(todo => { return todo.done })
    },
    pendings: function () {
      return this.todos.filter(todo => { return !todo.done })
    }
  }
}
</script>
