<template>
    <transition :name="transitionName" mode="out-in">
      <RouterView v-if="!loading" />
    </transition>
    <transition name="fade">
      <AnimatedSvg v-if="loading" />
    </transition>
</template>

<script setup>
import { ref, onMounted } from 'vue';
import { RouterLink, RouterView } from 'vue-router';
import AnimatedSvg from './components/animation/AnimatedSvg.vue';

const loading = ref(true);

onMounted(() => {
  initSnowify();
  // Simulate loading time
  setTimeout(() => {
    loading.value = false;
  }, 3500); // Adjust the time based on your animation duration
});
</script>
