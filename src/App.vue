<template>
  <Header msg="Welcome to Your Vue.js App"/>
  <BlogContent />
</template>

<script>
import Header from './components/Header.vue'
import BlogContent from './components/BlogContent.vue'

export default {
  name: 'App',
  components: {
    Header,
    BlogContent
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
}
</style>
