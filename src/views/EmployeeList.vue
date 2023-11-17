<template>
    <div>
      <h2>Employee List</h2>
      <div class="employee-list-container">
        <employee-list-item
          v-for="employee in employeeList"
          :key="employee.id"
          :name="employee.name"
          :avatar="employee.avatar"
          :position="employee.position"
        ></employee-list-item>
      </div>
    </div>
  </template>
  
  <script>
  import EmployeeListItem from '@/components/EmployeeListItem.vue';
  
  export default {
    name: 'EmployeeList',
    components: {
      EmployeeListItem,
    },
    data() {
      return {
        employeeList: [
          {
            id: 1,
            name: 'Employee 1',
            avatar: '@/assets/employee1-avatar.jpg',
            position: 'Position 1',
          },
          {
            id: 2,
            name: 'Employee 2',
            avatar: '@/assets/employee2-avatar.jpg',
            position: 'Position 2',
          },
          // Add more employees as needed
        ],
      };
    },
  };
  </script>