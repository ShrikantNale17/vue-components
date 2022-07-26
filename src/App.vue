<template>
  <!-- <GreetUser name="Bruce" heroName="Batman" />
  <GreetUser name="Clark" heroName="Superman" />
  <GreetUser name="Diana" heroName="Wonder woman" />
  <GreetUser :name="name" :heroName="channel" /> -->

  <!-- <ArticleComp
    id="my-article"
    title="Article title"
    :likes="50"
    :isPublished="true"
  /> -->

  <h2>AppComponent</h2>
  <h3>AppComponent username {{ name }}</h3>
  <ComponentC />
</template>

<script>
// import GreetUser from "./components/GreetUser.vue";
// import ArticleComp from "./components/ArticleComp.vue";
import ComponentC from "./components/ComponentC.vue";

export default {
  name: "App",
  components: {
    // GreetUser,
    // ArticleComp,
    ComponentC,
  },
  data() {
    return {
      name: "Shrikant",
      channel: "Codevolution",
    };
  },
  provide() {
    return {
      username: this.name,
    };
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
