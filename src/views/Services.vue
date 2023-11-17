<template>
    <div>
      <h2>Services</h2>
      <div class="service-container">
        <servicio-card
          v-for="service in services"
          :key="service.title"
          :title="service.title"
          :image="service.image"
          :description="service.description"
        ></servicio-card>
      </div>
    </div>
  </template>
  
  <script>
  import ServicioCard from '@/components/ServicioCard.vue';
  
  export default {
    name: 'Services',
    components: {
      ServicioCard,
    },
    data() {
      return {
        services: [
          {
            title: 'Service 1',
            image: '@/assets/service1.jpg',
            description: 'Description of Service 1.',
          },
          {
            title: 'Service 2',
            image: '@/assets/service2.jpg',
            description: 'Description of Service 2.',
          },
          {
            title: 'Service 3',
            image: '@/assets/service3.jpg',
            description: 'Description of Service 3.',
          },
        ],
      };
    },
  };
  </script>