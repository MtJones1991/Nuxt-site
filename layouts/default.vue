<template>
  <v-app dark>
    <div @click="tune">
        <nuxt/>
    </div>  
  </v-app>
</template>

<script>
import VueMoJS from 'vue-mo-js'
import mojs from 'mo-js'
  export default {
    data() {
      return {
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
        title: 'Vuetify.js',
        OPTS: {
              fill: 'none',
              radius: 55,
              strokeWidth: { 50 : 0 },
              scale: { 0: 1 },
              angle: { 'rand(-35, -70)': 0 },
              duration: 1500,
              left: 0, top: 0,
              easing: 'cubic.out'
            },
            circle1: undefined,
            circle2: undefined
        
      }
    },
    mounted () {
      this.circle1 = new mojs.Shape({
        ...this.OPTS,
        stroke: '#B71C1C',
      })
      
      this.circle2 = new mojs.Shape({
        ...this.OPTS,
        radius: { 0 : 15 },
        strokeWidth: { 30: 0 },
        stroke: 'orange',
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



</style>

