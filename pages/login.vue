<template>
  <div>
    <p v-if="$route.query.error">Something went wrong.</p>
    <p v-else-if="!$auth.loggedIn && !$route.query.code">Redirecting...</p>
    <p v-else>Logging In...</p>
  </div>
</template>
<script>
export default {
  name: 'LoginPage',

  created() {
    if (!this.$auth.loggedIn && !this.$route.query.code) {
      this.$auth.loginWith('spotify')
    }

    if (this.$route.query.error) {
      this.$router.push({ path: '/' })
    }
  },
}
</script>
