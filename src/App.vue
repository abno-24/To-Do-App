<script>
import ToDo from './components/ToDo.vue';

export default {
    setup() {
        components: {
            ToDo;
        }
    },
    components: { ToDo }
}
</script>

<template>
  <div id="app">
    <ToDo />
  </div>
</template>

<style>
</style>
