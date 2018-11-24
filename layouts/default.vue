<template>
  <v-app dark @click="tune">
        <nuxt />  
  </v-app>
</template>

<script>
import VueMoJS from 'vue-mo-js'
import mojs from 'mo-js'
  export default {
    data() {
      return {
           OPTS: {
      fill: 'none',
      radius: 25,
      strokeWidth: { 50 : 0 },
      scale: { 0: 1 },
      angle: { 'rand(-35, -70)': 0 },
      duration: 500,
      left: 0, top: 0,
      easing: 'cubic.out'
    },
    circle1: undefined,
    circle2: undefined,
        icons: [
          'fab fa-facebook',
          'fab fa-twitter',
          'fab fa-google-plus',
          'fab fa-linkedin',
          'fab fa-instagram'
        ],
        clipped: false,
        drawer: true,
        fixed: false,
        items: [
          { icon: 'apps', title: 'Welcome', to: '/' },
          { icon: 'bubble_chart', title: 'Inspire', to: '/inspire' }
        ],
        miniVariant: false,
        right: true,
        rightDrawer: false,
        title: 'Vuetify.js'
      }
    },
      mounted () {
    this.circle1 = new mojs.Shape({
      ...this.OPTS,
      stroke: 'cyan',
    })
    
    this.circle2 = new mojs.Shape({
      ...this.OPTS,
      radius: { 0 : 15 },
      strokeWidth: { 30: 0 },
      stroke: 'magenta',
      delay: 'rand(75, 150)'
    })
  },

  methods: {
    tune (e) {
      this.circle1
        .tune({ x: e.pageX, y: e.pageY })
        .replay();

      this.circle2
        .tune({ x: e.pageX, y: e.pageY })
        .replay();
    }
  }
  }
</script>

<style>
.page-enter-active, .page-leave-active {
    transition: all 1.5s;
}

.page-enter, .page-leave-active {
    opacity: 0;
    transform: scale(1);
}

body, html {
  padding: 0;
}

body {
  background: rgba(241, 226, 215, 0.2);
  background: #333;
}

#app div {
  width: 100vw;
  height: 100vh;
}


</style>
