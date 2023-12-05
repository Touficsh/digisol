<template>
  <div>
    <RouterView v-if="!loading" />
    <AnimatedSvg v-if="loading" />
  </div>
</template>

<script setup>
import { ref, onMounted } from 'vue';
import { RouterLink, RouterView } from 'vue-router';
import AnimatedSvg from './components/animation/AnimatedSvg.vue';

const loading = ref(true);

onMounted(() => {
  // Simulate loading time
  setTimeout(() => {
    loading.value = false;
  }, 4000); // Adjust the time based on your animation duration
});
</script>
