<template>
  <div class="home has-background-white-ter">
    <my-navbar></my-navbar>
    <div class="section">
      <figure class="image is-128x128">
        <img v-bind:src="user.photoURL" />
      </figure>
      <div class="container">{{ user.displayName }}</div>
    </div>
  </div>
</template>

<script>
import firebase from "firebase";
import MyNavbar from "@/components/MyNavbar.vue";

export default {
  name: "home",
  components: {
    MyNavbar
  },
  data: function() {
    return {
      user: firebase.auth().currentUser
    };
  }
};
</script>
