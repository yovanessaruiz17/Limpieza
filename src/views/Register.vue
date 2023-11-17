<template>
    <div>
      <h2>Register</h2>
      <form @submit.prevent="register">
        <!-- Agrega los campos según tus requisitos -->
        <label for="name">Name:</label>
        <input type="text" id="name" v-model="name" />
  
        <label for="email">Email:</label>
        <input type="email" id="email" v-model="email" />
  
        <label for="password">Password:</label>
        <input type="password" id="password" v-model="password" />
  
        <button type="submit">Register</button>
      </form>
    </div>
  </template>
  
  <script>
  export default {
    name: 'Register',
    data() {
      return {
        name: '',
        email: '',
        password: '',
      };
    },
    methods: {
      register() {
        // Implementa la lógica de registro
        console.log('Register:', this.name, this.email, this.password);
      },
    },
  };
  </script>