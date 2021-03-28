<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    <SelectUsername/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue';
// eslint-disable-next-line no-unused-vars
import SelectUsername from './components/SelectUsername.vue';

export default {
  name: 'App',
  components: {
    HelloWorld,
    SelectUsername,
  },
  data() {
    return {
      usernameAlreadySelected: false,
    };
  },
  methods: {
    // eslint-disable-next-line no-unused-vars
    onUsernameSelection(username) {
      this.usernameAlreadySelected = true;
    },
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
