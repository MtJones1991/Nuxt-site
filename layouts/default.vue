<template>
  <v-app dark>
        <nuxt />  
  </v-app>
</template>

<script>
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
        title: 'Vuetify.js'
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


</style>
