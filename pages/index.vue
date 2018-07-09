<template>
  <section class="container">
    <h1 class="h1">居酒屋GO的なアプリ</h1>
    <b-button variant="primary" @click="handleLineLogin">LINEではじめる</b-button>
    <b-button variant="primary" @click="handleTwitterLogin">Twitterではじめる</b-button>
    <b-button variant="primary" @click="handleFacebookLogin">Facebookではじめる</b-button>
  </section>
</template>

<script>
  import { lineLogin, twitterLogin, facebookLogin } from 'assets/js/auth.js';

  export default {
    methods: {
      handleLineLogin() {
        lineLogin();
      },
      handleTwitterLogin() {
        twitterLogin();
      },
      handleFacebookLogin() {
        facebookLogin();
      },
    },

  }

</script>
