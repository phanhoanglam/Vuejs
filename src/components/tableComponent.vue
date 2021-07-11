<template>
  <div class="table-component">
    <table>
      <tr>
        <th>Name</th>
        <th>Age</th>
        <th>Salary</th>
      </tr>
      <tr v-for="(user, index) in users" v-bind:key="index">
        <td>{{ user.name }}</td>
        <td>{{ user.age }}</td>
        <td>{{ user.salary }}</td>
      </tr>
    </table>
  </div>
</template>

<script>
export default {
  name: "table-component",
  props: {
    users: {
      name: String,
      age: Number,
      salary: Number,
    },
  },
  data() {
    return {};
  },
};
</script>

<style lang="css" scoped>
.table-component {
  width: 50%;
}
table {
  font-family: arial, sans-serif;
  border-collapse: collapse;
  width: 100%;
}

td,
th {
  border: 1px solid #dddddd;
  text-align: left;
  padding: 8px;
}

tr:nth-child(even) {
  background-color: #dddddd;
}
</style>