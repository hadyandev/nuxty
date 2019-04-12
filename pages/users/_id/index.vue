<template>
  <section class="container">
    <h1>User Detail - {{$route.params.id}}</h1>
    <p class="subheading">This User Detail Page</p>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Aliquid tempora libero pariatur accusamus, aut ratione doloremque, quas maxime minima praesentium, provident aspernatur molestiae. Debitis nisi quisquam minima, nesciunt magni beatae.</p>
  </section>
</template>

<script>
export default {
  head() {
    return {
      title: "About Nuxt",
      meta: [
        { name: "description", content: "This is my about description here." },
        { name: "keywords", content: "about nuxt, nuxt info" }
      ]
    };
  },
  validate(context) {
    //   return blank page if id is not number
    return /^\d+$/.test(context.params.id);
  }
};
</script>

<style>
</style>
