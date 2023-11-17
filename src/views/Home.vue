<template>
    <div>
      <h2>Home</h2>
      <div>
        <img src="@/assets/home-image.jpg" alt="Home Image" />
        <p>Informative paragraph about your home page.</p>
        <router-link to="/services">
          <button>Go to Services</button>
        </router-link>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'Home',
  };
  </script>