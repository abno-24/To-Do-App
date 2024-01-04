<script>
import Header from './components/Header.vue';
import ToDo from './components/ToDo.vue';

export default {
    setup() {
    },
    components: { ToDo, Header }
}
</script>

<template>
  <div id="app">
    <Header />
    <ToDo />
  </div>
</template>

<style>
</style>
