<template>
    <div class="service-card">
      <img :src="image" :alt="title" />
      <p>{{ description }}</p>
    </div>
  </template>
  
  <script>
  export default {
    name: 'ServicioCard',
    props: {
      title: String,
      image: String,
      description: String,
    },
  };
  </script>
  
  <style scoped>
  /* Agrega estilos según sea necesario */
  .service-card {
    border: 1px solid #ccc;
    padding: 10px;
    margin: 10px;
    text-align: center;
  }
  
  .service-card img {
    width: 100%;
    max-height: 150px;
    object-fit: cover;
  }
  </style>