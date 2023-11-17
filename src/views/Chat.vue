<template>
    <div>
      <h2>Chat</h2>
      <div class="chat-container">
        <chat-message
          v-for="message in chatMessages"
          :key="message.id"
          :isClient="message.isClient"
          :name="message.name"
          :avatar="message.avatar"
          :message="message.message"
        ></chat-message>
      </div>
    </div>
  </template>
  
  <script>
  import ChatMessage from '@/components/ChatMessage.vue';
  
  export default {
    name: 'Chat',
    components: {
      ChatMessage,
    },
    data() {
      return {
        chatMessages: [
          {
            id: 1,
            isClient: true,
            name: 'Client Name',
            avatar: '@/assets/client-avatar.png',
            message: 'Hello, how can I help you?',
          },
          {
            id: 2,
            isClient: false,
            name: 'Employee Name',
            avatar: '@/assets/employee-avatar.jpg',
            message: 'Hi! Im here to assist you.',
          },
          // Add more messages as needed
        ],
      };
    },
  };
  </script>