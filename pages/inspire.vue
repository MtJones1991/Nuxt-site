<template>
  <div>
      <v-layout align-center justify-center column fill-height>
      <h1 class="mt-3 mb-5">Home</h1>
      <v-btn color="warning" class="mt-3 mb-5">
        <nuxt-link to="/">Home</nuxt-link>
      </v-btn>
        <!-- <Logo/> -->
      </v-layout>
  <BottomNav/>
  </div>
</template>

<script>
import BottomNav from '~/components/BottomNav.vue'
import VueMoJS from 'vue-mo-js'

  export default {
    components: {
      BottomNav
    },
  }
</script>

<style lang="stylus">
  .custom-ripple
    user-select: none

  .cardA {
    border-radius: 100%;
  }
</style>
