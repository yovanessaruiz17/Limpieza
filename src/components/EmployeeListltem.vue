<template>
    <div class="employee-list-item">
      <img :src="avatar" :alt="name" />
      <div>
        <h3>{{ name }}</h3>
        <p>{{ position }}</p>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'EmployeeListItem',
    props: {
      name: String,
      avatar: String,
      position: String,
    },
  };
  </script>
  
  <style scoped>
  /* Agrega estilos según sea necesario */
  .employee-list-item {
    display: flex;
    align-items: center;
    margin-bottom: 10px;
  }
  
  .employee-list-item img {
    width: 50px;
    height: 50px;
    border-radius: 50%;
    margin-right: 10px;
  }
  </style>