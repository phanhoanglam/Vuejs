<template>
  <div class="header">
    <h3>{{ title }}</h3>
  </div>
</template>

<script>
export default {
  name: "header-component",
  data() {
    return {
      title: "Employee Management",
    };
  },
};
</script>

<style>
.header {
  overflow: hidden;
  background-color: #f1f1f1;
  padding: 20px 10px;
}
</style>