<template>
    <div class="user-history-card">
      <img :src="image" :alt="name" />
      <p>{{ description }}</p>
      <div class="rating">
        <span v-for="n in rating" :key="n">⭐</span>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'UserHistoryCard',
    props: {
      name: String,
      image: String,
      description: String,
      rating: Number,
    },
  };
  </script>
  
  <style scoped>
  /* Agrega estilos según sea necesario */
  .user-history-card {
    border: 1px solid #ccc;
    padding: 10px;
    margin: 10px;
    text-align: center;
  }
  
  .user-history-card img {
    width: 100%;
    max-height: 150px;
    object-fit: cover;
  }
  
  .rating {
    margin-top: 10px;
  }
  </style>