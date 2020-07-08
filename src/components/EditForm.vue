<template>
  <div class="edit-form">
    <input type="text" :value="message" @input="doUpdate" >
  </div>
</template>

<script>
export default {
  name: 'EditForm',
  components: {},
  computed: {
    message: function () {
      return this.$store.getters.message;
    },
  },
  methods: {
    doUpdate: function (event) {
      this.$store.dispatch('doUpdate', event.target.value);
    },
  },
};
</script>