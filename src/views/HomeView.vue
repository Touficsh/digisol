<script>
import { defineComponent } from 'vue'
import NavBar from '../components/NavBar.vue'
import PageHeader from '../components/PageHeader.vue'
import Features from '../components/Features.vue'
import Services from '../components/Services.vue'
import Pricing from '../components/Pricing.vue'
import Projects from '../components/Projects.vue'

export default defineComponent({
 components: {
   NavBar,
   PageHeader,
   Features,
   Services,
   Pricing,
   Projects,
 } 
})
</script>

<template>
  <main class="presentation-page">
    <NavBar />
    <PageHeader />
    <Features />
    <Services />
    <Pricing />
    <Projects />
  </main>
</template>
