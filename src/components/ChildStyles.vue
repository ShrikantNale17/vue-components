<template>
  <div>
    <h4>Child Styles Component</h4>
    <slot></slot>
  </div>
</template>

<script>
export default {
  name: "ChildStyles",
};
</script>

<style scoped>
h4 {
  color: olive;
}
</style>
