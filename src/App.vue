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

  <!-- <CardComp>Card content</CardComp>
  <CardComp><h2>Card content</h2></CardComp>
  <CardComp><img src="https://picsum.photos/200" alt="" /></CardComp>
  <card-comp>
    <template v-slot:header>
      <h2>Header</h2>
    </template>
    <template v-slot:default>
      <img src="https://picsum.photos/200/300" alt="" />
    </template>
    <template v-slot:footer>
      <button>View details</button>
    </template>
  </card-comp> -->

  <!-- <NameList>
    <template v-slot:default="slotProps">
      {{ slotProps.firstName }} {{ slotProps.lastName }}
    </template>
  </NameList>

  <NameList>
    <template v-slot:default="slotProps">
      {{ slotProps.lastName }} {{ slotProps.firstName }}
    </template>
  </NameList>

  <NameList>
    <template v-slot:default="slotProps">
      {{ slotProps.firstName }}
    </template>
  </NameList> -->

  <!-- <h4>Parent Style Component</h4>
  <ChildStyles>
    <h4>Childs slot style</h4>
  </ChildStyles> -->

  <button @click="activeTab = 'TabA'">Tab A</button>
  <button @click="activeTab = 'TabB'">Tab B</button>
  <button @click="activeTab = 'TabC'">Tab C</button>
  <component :is="activeTab"></component>
</template>

<script>
// import GreetUser from "./components/GreetUser.vue";
// import ArticleComp from "./components/ArticleComp.vue";
// import PopUp from "./components/PopUp.vue";
// import InputComp from "./components/InputComp.vue";
// import CardComp from "./components/CardComp.vue";
// import NameList from "./components/NameList.vue";
// import ChildStyles from "./components/ChildStyles.vue";
import TabA from "./components/TabA.vue";
import TabB from "./components/TabB.vue";
import TabC from "./components/TabC.vue";

export default {
  name: "App",
  components: {
    // GreetUser,
    // ArticleComp,
    // ComponentC,
    // PopUp,
    // InputComp,
    // CardComp,
    // NameList,
    // ChildStyles,
    TabA,
    TabB,
    TabC,
  },
  data() {
    return {
      //   showPopup: false,
      //   name: "",
      activeTab: "TabA",
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

<style scoped>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 20px;
}

h4 {
  color: orange;
}
</style>
