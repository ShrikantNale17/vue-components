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

  <!-- <h2>AppComponent</h2>
  <h3>AppComponent username {{ name }}</h3>
  <ComponentC /> -->

  <!-- <button @click="showPopup = true">Show PopUp</button>
  <PopUp v-show="showPopup" @close="closePopup" /> -->

  <!-- <InputComp v-model="name" /> -->

  <CardComp>Card content</CardComp>
  <CardComp><h2>Card content</h2></CardComp>
  <CardComp><img src="https://picsum.photos/200" alt="" /></CardComp>
</template>

<script>
// import GreetUser from "./components/GreetUser.vue";
// import ArticleComp from "./components/ArticleComp.vue";
// import PopUp from "./components/PopUp.vue";
// import InputComp from "./components/InputComp.vue";
import CardComp from "./components/CardComp.vue";

export default {
  name: "App",
  components: {
    // GreetUser,
    // ArticleComp,
    // ComponentC,
    // PopUp,
    // InputComp,
    CardComp,
  },
  data() {
    return {
      //   showPopup: false,
      name: "",
    };
  },
  methods: {
    // closePopup(value) {
    //   this.showPopup = false;
    //   console.log(value);
    // },
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
