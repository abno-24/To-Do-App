<template>
  <div id="app" class="flex flex-col">
    <Header />
    <Info />
    <NewTask />
    <hr class="my-4 bg-white" />
    <div class="border-b-2 mb-2 border-gray-200 max-md:w-[98%]">
        <p class="italic font-extralight text-gray-400">Tasks</p>
    </div>
    <ul class="relative max-md:w-[90%] pb-8">
      <TaskList v-for="task in tasks" :key="task.id" :tasks="task" />
    </ul>
  </div>
</template>
<script setup>
import Header from './components/Header.vue';
import NewTask from './components/NewTask.vue';
import Info from './components/Info.vue';
import TaskList from './components/TaskList.vue'

const tasks = [
  {
    id: 1,
    name: "Gym",
  },
  {
    id: 2,
    name: "Meditation",
  },
  {
    id: 3,
    name: "Journal Writing",
  },
  {
    id: 4,
    name: "Book Reading",
  },
]

components: { Header, NewTask, Info, TaskList }
</script>

<style></style>
