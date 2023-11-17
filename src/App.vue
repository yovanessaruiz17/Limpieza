<template>
  <div id="app">
    <nav>
        <img src="@/assets/logo.png" alt="Logo" />
        <router-link to="/">Home</router-link>
        <router-link to="/services">Services</router-link>
        <router-link to="/user-history">User History</router-link>
        <router-link to="/contact">Contact</router-link>
        <router-link to="/login">Login</router-link>
        <router-link to="/register">Register</router-link>
    </nav>
    <router-view />
    <footer>
      <!-- Términos y condiciones -->
      <p>Terms and Conditions</p>
      <!-- Redes sociales -->
      <div>
        <a href="#">Facebook</a>
        <a href="#">Twitter</a>
        <a href="#">Instagram</a>
      </div>
    </footer>
  </div>
</template>

<script>
import Home from './views/Home.vue';

export default {
  name: 'App',
  components:{Home}
};
</script>

<style>

</style>
