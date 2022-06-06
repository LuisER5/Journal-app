<template>
  <img alt="Vue logo" src="../assets/logo.png" />

  <h1>Hola mundo</h1>
  
  <button @click="goToDaybook" type="button" class="btn btn-primary">
    Day book
  </button>
</template>

<script>
export default {
  name: "HomeView",

  methods: {
    goToDaybook() {
      this.$router.push({ name: "no-entry" });
    },
  },
};
</script>
