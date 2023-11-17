<template>
    <div>
      <h2>Login</h2>
      <form @submit.prevent="login">
        <label for="email">Email:</label>
        <input type="email" id="email" v-model="email" />
  
        <label for="password">Password:</label>
        <input type="password" id="password" v-model="password" />
  
        <button type="submit">Login</button>
      </form>
    </div>
  </template>
  
  <script>
  export default {
    name: 'Login',
    data() {
      return {
        email: '',
        password: '',
      };
    },
    methods: {
      login() {
        // Implementa la lógica de inicio de sesión
        console.log('Login:', this.email, this.password);
      },
    },
  };
  </script>