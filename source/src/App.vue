<template>
  <div id="app">
    <a-layout>
      <my-header></my-header>
      <my-jumbotron></my-jumbotron>
      <my-content></my-content>
      <my-footer></my-footer>
    </a-layout>
  </div>
</template>

<script>
import header from "./components/header"
import jumbotron from "./components/jumbotron"
import content from "./components/content"
import footer from "./components/footer"
export default {
  name: 'app',
  components: {
    "my-header": header,
    "my-jumbotron": jumbotron,
    "my-content": content,
    "my-footer": footer
  }
}
</script>

<style lang="scss">
ul, li, a{
  text-decoration: none;
  list-style: none;
  margin: 0;
  padding: 0;
}
  
</style>
