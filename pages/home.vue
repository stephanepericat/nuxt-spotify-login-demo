<template>
  <div class="home-view">
    <h3
      class="text-title-small"
      v-text="`Welcome, ${$auth.user.display_name}!`"
    />
  </div>
</template>
<script>
export default {
  name: 'HomeView',
}
</script>
