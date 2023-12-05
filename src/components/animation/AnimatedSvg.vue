<!-- AnimatedSVG.vue -->
<template>
  <div class="d-flex align-items-center justify-content-center animation">
    <svg width="200" height="200" xmlns="http://www.w3.org/2000/svg">
      <!-- Your SVG content here -->
      <circle cx="100" cy="100" r="60" stroke="black" stroke-width="3" fill="red" class="animated-circle"></circle>
    </svg>
  </div>
</template>

<script>
export default {
  mounted() {
    // Add animation logic here (CSS or JavaScript)
  }
};
</script>

<style scoped>
/* Add your CSS animation styles here */
@keyframes bounce {
  0%, 20%, 50%, 80%, 100% {
    transform: translateY(0);
  }
  40% {
    transform: translateY(-30px);
  }
  60% {
    transform: translateY(-15px);
  }
}

.animation {
  height: 100vh;
}
.animated-circle {
  animation: bounce 2s infinite;
}
</style>
