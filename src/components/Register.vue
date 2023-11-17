<template>
    <div>
      <h2>Register</h2>
      <form>
        <!-- Agrega los campos según tus requisitos -->
        <label for="name">Name:</label>
        <input type="text" id="name" v-model="name" />
  
        <!-- Agrega más campos aquí -->
  
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
        // Agrega más variables según sea necesario
      };
    },
  };
  </script>