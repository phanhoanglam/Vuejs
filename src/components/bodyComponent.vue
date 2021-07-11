<template>
  <!-- <div>Body component</div> -->
  <table-component v-bind:users="users"></table-component>
</template>

<script>

import tableComponent from "./tableComponent.vue"
export default {
  name: "body-component",
  data() {
    return {
      users: [
        {
          name: "Wiliam",
          age: 25,
          salary: 2000,
        },
        {
          name: "Adela",
          age: 27,
          salary: 2000,
        },
        {
          name: "Lisa",
          age: 22,
          salary: 2000,
        },
        {
          name: "Angela",
          age: 25,
          salary: 2000,
        },
      ],
    };
  },
  components: {
    tableComponent
  }
};
</script>

<style>
</style>