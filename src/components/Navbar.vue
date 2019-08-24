<template>
  <header>
    <nav class="navbar has-shadow is-danger is-fixed-top" role="navigation" aria-label="main navigation">
      <div class="navbar-brand">
        <a class="navbar-item" href="https://bulma.io">
          <!--img src="https://bulma.io/images/bulma-logo.png" width="112" height="28" /-->
          <div class="has-text-light"><strong>LOGO</strong> | nomedaapp</div>
        </a>

        <a
          role="button"
          class="navbar-burger burger"
          aria-label="menu"
          aria-expanded="false"
          data-target="navbarBasicExample"
        >
          <span aria-hidden="true"></span>
          <span aria-hidden="true"></span>
          <span aria-hidden="true"></span>
        </a>
      </div>

      <div id="navbarBasicExample" class="navbar-menu">
        <div class="navbar-end">
          <a class="navbar-item has-text-light">Home</a>
          <a class="navbar-item has-text-light">Como funciona</a>
          <a class="navbar-item has-text-light">Contato</a>
        </div>
      </div>
    </nav>
  </header>
</template>

<script>
export default {
  name: 'navbar'
}
</script>

<style scoped>
  .navbar {
    background-image: linear-gradient(-90deg, #361A43, #674299);
  }
</style>
