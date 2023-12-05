<template>
  <main>
    <div>
      <NavBar @scroll="scrollToElement" />
    </div>
    <div ref="PageHeader">
      <PageHeader  />
    </div>
    <div ref="Features">
      <Features  />
    </div>
    <!-- <div ref="Services">
      <Services  />
    </div> -->
    <div ref="Pricing">
      <Pricing  />
    </div>
    <div ref="Projects">
      <Projects  />
    </div>
    <div ref="Contact-us">
      <ContactUs  />
    </div>
  </main>
</template>

<script>
import { defineComponent } from 'vue'
import NavBar from '../components/NavBar.vue'
import PageHeader from '../components/PageHeader.vue'
import Features from '../components/Features.vue'
import Services from '../components/Services.vue'
import Pricing from '../components/Pricing.vue'
import Projects from '../components/Projects.vue'
import ContactUs from '../components/ContactUs.vue'

export default defineComponent({
 components: {
   NavBar,
   PageHeader,
   Features,
   Services,
   Pricing,
   Projects,
   ContactUs
 },
 methods: {
    scrollToElement(value) {
      const scroll = this.$refs[value];
      if (scroll) {
        scroll.scrollIntoView({ behavior: "smooth" });
      }
    },
  },
})
</script>

