<template>
    <div class="chat-message" :class="{ 'client-message': isClient, 'employee-message': !isClient }">
      <img :src="avatar" :alt="name" />
      <div>
        <p>{{ message }}</p>
        <span>{{ name }}</span>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'ChatMessage',
    props: {
      isClient: Boolean,
      name: String,
      avatar: String,
      message: String,
    },
  };
  </script>
  
  <style scoped>
  /* Agrega estilos según sea necesario */
  .chat-message {
    display: flex;
    align-items: center;
    margin-bottom: 10px;
  }
  
  .client-message {
    justify-content: flex-start;
  }
  
  .employee-message {
    justify-content: flex-end;
  }
  
  .chat-message img {
    width: 40px;
    height: 40px;
    border-radius: 50%;
    margin-right: 10px;
  }
  </style>