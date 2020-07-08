<template>
  <div class="edit-form">
    <input v-model="message">
  </div>
</template>

<script>
export default {
  name: 'EditForm',
  components: {},
  computed: {
    message: {
      get() { return this.$store.getters.message; },
      set(value) { this.$store.dispatch('doUpdate', event.target.value); }
    },
  },
};
</script>