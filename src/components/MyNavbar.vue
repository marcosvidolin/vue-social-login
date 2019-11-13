<template>
  <nav class="navbar" role="navigation" aria-label="main navigation">
    <div class="navbar-brand">
      <a class="navbar-item" href="https://bulma.io">
        <img src="https://bulma.io/images/bulma-logo.png" width="112" height="28" />
      </a>

      <a
        id="example-burger"
        role="button"
        class="navbar-burger burger"
        aria-label="menu"
        aria-expanded="false"
        data-target="main-menu"
      >
        <span aria-hidden="true"></span>
        <span aria-hidden="true"></span>
        <span aria-hidden="true"></span>
      </a>
    </div>

    <div id="main-menu" class="navbar-menu">
      <div class="navbar-end">
        <div class="navbar-item">
          <a
            class="button"
            href="https://github.com/marcosvidolin/vue-social-login"
            target="_blank"
          >
            <i class="fab fa-github"></i> &nbsp; Github
          </a>
        </div>
        <div class="navbar-item">
          <div class="buttons" @click="logout">
            <a class="button is-outlined is-danger">Logout</a>
          </div>
        </div>
      </div>
    </div>
  </nav>
</template>

<script>
import firebase from "firebase";

export default {
  name: "my-navbar",
  methods: {
    logout: function() {
      firebase
        .auth()
        .signOut()
        .then(() => {
          this.$router.replace("login");
        });
    }
  },
  mounted: function() {
    var burger = document.getElementById("example-burger");
    var menu = document.getElementById("main-menu");
    burger.addEventListener("click", function() {
      burger.classList.toggle("is-active");
      menu.classList.toggle("is-active");
    });
  }
};
</script>