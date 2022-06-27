<template>
  <div class="container">
    <h1>{{message}}</h1>
  </div>
</template>

<script>
import {messages} from './json.js';
export default {
  name: 'App',
  components: {
  },
  data() {
    return {
      messages,
      message : messages[Math.floor(Math.random() * messages.length)]
    }
  },
  methods : {
    
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
