<template>
  <div>
    <h2>PopUp Component</h2>
    <button @click="$emit('close', 'Shrikant')">Close PopUp</button>
  </div>
</template>

<script>
export default {
  name: "PopUp",
  emits: ["close"],
};
</script>

<style scoped></style>
