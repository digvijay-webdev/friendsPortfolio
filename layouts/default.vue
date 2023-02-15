<template>
  <v-app dark>
    <!-- Cube animations -->
    <div class="parent">
      <div class="cube"></div>
      <div class="cube"></div>
      <div class="cube"></div>
      <div class="cube"></div>
      <div class="cube"></div>

      <Navbar />
      <Nuxt />
    </div>
  </v-app>
</template>

<script>
import Navbar from "@/components/Navbar.vue";

export default {
  name: 'DefaultLayout',
  components: {
    Navbar
  },
  data () {
    return {}
  }
}
</script>

<style lang="scss">
.parent {
  background-color: transparent;
  position: relative;
  height: 100%;
  overflow: hidden;
  font-family: 'Montserrat', sans-serif;
}

.cube {
  position: absolute;
  top: 80vh;
  left: 45vw;
  width: 10px;
  height: 10px;
  border: solid 1px darken(#636e72cc, 8%);
  transform-origin: top left;
  transform: scale(0) rotate(0deg) translate(-50%, -50%);
  animation: cube 12s ease-in forwards infinite;
  
  &:nth-child(2n) {
    border-color: lighten(#636e72cc, 10%);
  }
  
  
  &:nth-child(3) {
    animation-delay: 4s;
    left: 75vw;
    top: 50vh;
  }
  
  &:nth-child(4) {
    animation-delay: 6s;
    left: 90vw;
    top: 10vh;
  }
  
  &:nth-child(5) {
    animation-delay: 8s;
    left: 10vw;
    top: 85vh;
  }
  
  &:nth-child(6) {
    animation-delay: 10s;
    left: 50vw;
    top: 10vh;
  }
}

@keyframes cube {
  from {
    transform: scale(0) rotate(0deg) translate(-50%, -50%);   
    opacity: 1;
  }
  to {
    transform: scale(10) rotate(960deg) translate(-50%, -50%); 
    opacity: 0;
  }
}
</style>
