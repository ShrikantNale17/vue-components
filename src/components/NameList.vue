<template>
  <h2 v-for="name in names" :key="name.firstName">
    <slot :firstName="name.firstName" :lastName="name.lastName"></slot>
  </h2>
</template>

<script>
export default {
  name: "NameList",
  data() {
    return {
      names: [
        {
          firstName: "Bruce",
          lastName: "Wayne",
        },
        {
          firstName: "Clark",
          lastName: "Kent",
        },
        {
          firstName: "Princess",
          lastName: "Diana",
        },
      ],
    };
  },
};
</script>

<style scoped></style>
