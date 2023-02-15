<template>
  <main>
    <Hero />
    <Experience />
    <Projects />
    <Credentials />
    <Footer />
  </main>
</template>

<script>
import Hero from "@/components/Hero.vue";
import Experience from "@/components/Experience.vue";
import Projects from "@/components/Projects.vue";
import Credentials from "@/components/Credentials.vue";
import Footer from "@/components/Footer.vue";

export default {
  name: 'IndexPage',
  components: {
    Hero,
    Experience,
    Projects,
    Credentials,
    Footer,
  }
}
</script>
