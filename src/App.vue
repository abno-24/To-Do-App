<template>
  <div id="app">
    <Header />
    <ToDo />
    <Info />
    <div v-for="task in tasks" :key="task">
      <p>task</p>
    </div>
  </div>
</template>
<script>
import Header from './components/Header.vue';
import ToDo from './components/ToDo.vue';
import Info from './components/Info.vue';

export default {
    setup() {
      const tasks = [
        {
          id: 1,
          name: "Gym",
        },
        {
          id: 2,
          name: "Book Reading",
        },
      ]

      return tasks;
    },
    components: { Header, ToDo, Info }
}
</script>

<style>
</style>
