<template>
  <p>Please wait...</p>
</template>

<script>
import firebase from "firebase";

export default {
  name: "instagram-login",
  methods: {
    /**
     * Returns the ID of the Firebase project.
     */
    getFirebaseProjectId: function() {
      return firebase.app().options.authDomain.split(".")[0];
    },
    /**
     * This callback is called by the JSONP callback of the 'token' Firebase Function with the Firebase auth token.
     */
    tokenReceived: function(data) {
      if (data.token) {
        firebase
          .auth()
          .signInWithCustomToken(data.token)
          .then(function() {
            this.$router.replace("home");
          });
      } else {
        console.error(data);
        document.body.innerText = "Error in the token Function: " + data.error;
      }
    }
  },
  beforeMount() {
    let code = this.$route.query.code;
    let state = this.$route.query.state;
    let error = this.$route.query.error;
    if (error) {
      document.body.innerText = "Error back from the Instagram auth page: " + error;
    } else if (!code) {
      // Start the auth flow.
      window.location.href = "https://us-central1-" + this.getFirebaseProjectId() + ".cloudfunctions.net/redirect";
    } else {
      alert('caiu no else');
      // Use JSONP to load the 'token' Firebase Function to exchange the auth code against a Firebase custom token.
      const script = document.createElement("script");
      script.type = "text/javascript";
      // This is the URL to the HTTP triggered 'token' Firebase Function.
      // See https://firebase.google.com/docs/functions.
      let tokenFunctionURL = "https://us-central1-" + this.getFirebaseProjectId() + ".cloudfunctions.net/token";
      script.src = tokenFunctionURL + "?code=" + code + "&state=" +
        state + "&callback=" + this.tokenReceived.name;
        alert(script);
      document.head.appendChild(script);
    }
  }
};
</script>