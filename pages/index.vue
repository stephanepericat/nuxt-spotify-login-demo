<template>
  <div class="spotify-client">
    <button v-if="!$auth.loggedIn" @click="$auth.loginWith('spotify')">
      Login with Spotify
    </button>
    <div v-else>Welcome, {{ $auth.user.display_name }}!</div>
  </div>
</template>

<script>
export default {
  name: 'IndexPage',

  auth: false,
}
</script>
