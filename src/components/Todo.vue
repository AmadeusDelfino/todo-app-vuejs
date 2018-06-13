<template>
    <div class=card>
        <div class="header">
          {{ todo.title }} <span class="btn">Editar</span>
        </div>
        <div class="body">
          {{ todo.project }}
        </div>
        <div class="check">
          <input
          type="checkbox"
          v-model="todo.done"
          >
        </div>
      </div>
</template>

<script>
export default {
  props: ['todo']
}
</script>

<style scoped>
  .card {
    background-color: beige;
    margin: 10px;
    padding: 10px;
  }

  .card > .header {
    background-color: blanchedalmond;
    padding: 5px;
  }

  .card > .body {
    background-color: azure;
    padding: 5px;
  }

  .card > .check{
    background: white;
    padding: 5px;
  }

  .btn {
    background-color: grey;
    padding: 3px;
    cursor: pointer;
  }

  .btn:hover {
    background-color: #545454;
    color: white;
  }
</style>
