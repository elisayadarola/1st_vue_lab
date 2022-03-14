<template>
<div id="app">
  <lab/> 
  <button @click="helloWorld">Button</button>
  <p>{{Text}}</p>
  </div>
</template>

<script>
import lab from './components/lab.vue';

export default {
  data () {
    return {
    Text: "This is a text"
    }
  },
  components: {
    lab,
  },
  methods: {
    helloWorld() {
      console.log('Hello World');
    }
  }
}
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
