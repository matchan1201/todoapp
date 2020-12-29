<template>
  <div id="app">
    <ul>
      <li v-for="todo in todos" :key='todo'> <!--v-forを使う際は、keyを指定する -->
        <span>{{ todo.text }}</span>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'app',
  data() {
    return {
      todos: [
        { id: 1, text: 'dataを表示する' },
        { id: 2, text: 'ディレクティブを知る' },
      ],
    }
  }
}
</script>

<style>
</style>
