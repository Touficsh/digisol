<!-- AnimatedSVG.vue -->
<template>
    <div class="d-flex justify-center align-center abc">
      <transition name="fade">
        <img class="responsive-gif" src="../../assets/img/digisol.webp" alt="Entrance GIF">
      </transition>
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
.abc {
  height: 100vh;
  display: flex;
  align-items: center;
  align-content: center;
  justify-content: center;
  justify-items: center;
}
.responsive-gif {
  margin: auto !important;
  height: max-content !important;
}
.fade-enter-active, .fade-leave-active {
  transition: opacity 0.5s;
}
.fade-enter, .fade-leave-to {
  opacity: 0;
}
</style>
