<template>
  <div>
    <h2>Article Component</h2>
    <h3 v-bind="$attrs">{{ title }}</h3>
    <h3>Likes - {{ likes }}</h3>
    <h3>Published - {{ isPublished ? "Yes" : "No" }}</h3>
  </div>
</template>

<script>
export default {
  name: "ArticleComp",
  props: {
    title: {
      type: String,
      required: true,
      default: "Article default title",
    },
    likes: Number,
    isPublished: Boolean,
  },
  inheritAttrs: false,
};
</script>

<style scoped></style>
