<template>
  <section class="container">
    <h1>Nuxt User</h1>
    <p class="subheading">Find User!</p>
    <input type="text" v-model="id">
    <button @click="loadUser">Load User</button>
  </section>
</template>

<script>
export default {
  head() {
    return {
      title: "Users",
      meta: [
        { name: "description", content: "This is user page" },
        { name: "keywords", content: "search the user" }
      ]
    };
  },
  data() {
    return { id: "" };
  },
  methods: {
    loadUser() {
      this.$router.push(`/users/${this.id}`);
    }
  }
};
</script>

<style>
</style>
