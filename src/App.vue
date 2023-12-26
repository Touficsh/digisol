<template>
    <Transition name="slide-up">
      <AnimatedSvg v-if="loading" />
    </Transition>
    <RouterView v-if="!loading" />
</template>

<script setup>
import { ref, onMounted } from 'vue';
import { RouterLink, RouterView } from 'vue-router';
import AnimatedSvg from './components/animation/AnimatedSvg.vue';

const loading = ref(true);

onMounted(() => {
  // initSnowify();
  // Simulate loading time
  setTimeout(() => {
    loading.value = false;
  }, 2800); // Adjust the time based on your animation duration
});
</script>

<style>
.slide-up-enter-active {
  transition: transform 0.2s linear, opacity 0.3s linear;
}

.slide-up-leave-active {
  transition: transform 0.8s cubic-bezier(1, 0.5, 0.8, 1), opacity 0.8s cubic-bezier(1, 0.5, 0.8, 1);
}

.slide-up-enter-from,
.slide-up-leave-to {
  transform: translateY(-200px);
  opacity: 0;
}
</style>
