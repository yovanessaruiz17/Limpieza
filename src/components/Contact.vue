<template>
    <div>
      <h2>Contact</h2>
      <div>
        <img src="@/assets/contact-image.jpg" alt="Contact Image" />
        <p>Informative paragraph about contact.</p>
        <button @click="sendEmail">Contact via Email</button>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'Contact',
    methods: {
      sendEmail() {
        // Implementa la lógica para enviar correos electrónicos
      },
    },
  };
  </script>