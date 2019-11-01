<template>
  <div id="employee-table">
    <table>
      <thead>
        <tr>
          <th>Emoloyee name</th>
          <th>Employee email</th>
        </tr>
      </thead>
      <tbody>
        <tr v-for="employee in employees" :key="employee.id">
          <td>{{employee.name}}</td>
          <td>{{employee.email}}</td>
        </tr>
      </tbody>
    </table>
  </div>
</template>

<script>
export default {
  name: "employee-tale",
  props: {
    employees: Array
  }
};
</script>
<style scoped>
</style>