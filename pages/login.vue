<template>
  <div>Logging in...</div>
</template>
<script>
export default {
  name: 'LoginPage',

  mounted() {
    if(this.$route.query.error) {
      this.$router.push({ path: "/" });
    }
  }
}
</script>
