<template>
  <div id="app">
    <navbar></navbar>
  </div>
</template>

<script>
import Navbar from './components/Navbar'

export default {
  name: 'app',
  components: {
    Navbar
  }
}
</script>

<style>
@import "~bulma/css/bulma.css";
</style>
