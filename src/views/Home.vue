<template>
  <div class="home has-background-white-ter">
    <my-navbar></my-navbar>

    <div class="section">
      <div class="columns is-centered">
        <div class="column is-3">
          <div class="card">
            <header class="card-header">
              <p class="card-header-title">Authenticated User</p>
            </header>
            <div class="card-content">
              <div class="media">
                <div class="media-left">
                  <figure class="image is-48x48">
                    <img v-bind:src="user.photoURL" v-bind:alt="user.displayName"/>
                  </figure>
                </div>
                <div class="media-content">
                  <p class="title is-4">{{ user.displayName }}</p>
                  <p class="subtitle is-6">{{ user.email }}</p>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>      
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
