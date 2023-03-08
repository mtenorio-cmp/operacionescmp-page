<template>
  <div id="app">
    <HomeComponet />
  </div>
</template>

<script>
import HomeComponet from './components/home-component.vue';

export default {
  name: 'App',
  components: {
    HomeComponet,
  },
};
</script>

<style>
#app {
  font-family: 'Source Sans Pro', sans-serif;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
