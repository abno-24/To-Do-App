<script>
import Header from './components/Header.vue';
import ToDo from './components/ToDo.vue';
import Info from './components/Info.vue';

export default {
    setup() {
    },
    components: { Header, ToDo, Info }
}
</script>

<template>
  <div id="app">
    <Header />
    <ToDo />
    <Info />
  </div>
</template>

<style>
</style>
