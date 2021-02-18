<template>
  <div>
    <h1>Create an Event, {{ user.name }}</h1>
    <p>This event was created by {{ user.name }}</p>
  </div>
</template>

<script>
export default {
  computed: {
    user() {
      return {
        id: this.$store.state.user.id,
        name: this.$store.state.user.name,
      }
    },
  },
}
</script>