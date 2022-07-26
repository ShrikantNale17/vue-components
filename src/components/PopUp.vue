<template>
  <div>
    <h2>PopUp Component</h2>
    <input type="text" v-model="name" />
    <button @click="$emit('close', name)">Close PopUp</button>
  </div>
</template>

<script>
export default {
  name: "PopUp",
  emits: {
    close: (name) => {
      if (!name) {
        return false;
      } else {
        return true;
      }
    },
  },
  data() {
    return {
      name: "",
    };
  },
};
</script>

<style scoped></style>
