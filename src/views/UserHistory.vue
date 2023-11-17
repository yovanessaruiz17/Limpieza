<template>
    <div>
      <h2>User History</h2>
      <div class="user-history-container">
        <user-history-card
          v-for="userHistory in userHistories"
          :key="userHistory.name"
          :name="userHistory.name"
          :image="userHistory.image"
          :description="userHistory.description"
          :rating="userHistory.rating"
        ></user-history-card>
      </div>
    </div>
  </template>
  
  <script>
  import UserHistoryCard from '@/components/UserHistoryCard.vue';
  
  export default {
    name: 'UserHistory',
    components: {
      UserHistoryCard,
    },
    data() {
      return {
        userHistories: [
          {
            name: 'User 1',
            image: '@/assets/user1.jpg',
            description: 'Description of User 1.',
            rating: 4,
          },
          {
            name: 'User 2',
            image: '@/assets/user2.jpg',
            description: 'Description of User 2.',
            rating: 5,
          },
          {
            name: 'User 3',
            image: '@/assets/user3.jpg',
            description: 'Description of User 3.',
            rating: 3,
          },
          {
            name: 'User 4',
            image: '@/assets/user4.jpg',
            description: 'Description of User 4.',
            rating: 4.5,
          },
        ],
      };
    },
  };
  </script>