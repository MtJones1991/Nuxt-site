<template>
  <div>
      <v-layout align-center justify-center column fill-height>
      <h1 class="mt-3 mb-5">Home</h1>
      <v-btn color="warning" class="mt-3 mb-5">
        <nuxt-link to="/">Home</nuxt-link>
      </v-btn>
        <!-- <Logo/> -->
      </v-layout>

  <v-layout row>
    <v-flex xs12>
      <v-card
        :color="colors[color]"
        class="custom-ripple"
        ripple
        height="300"
        @mousemove="color = (color + 1) % colors.length"
      >
        <div class="title white--text pl-3 pt-3">{{ colors[color] }}</div>
      </v-card>
    </v-flex>
  </v-layout>

  </div>
</template>

<script>
  export default {
    data () {
      return {
        color: 0,
        colors: [
          'red',
          'pink',
          'purple',
          'deep-purple',
          'indigo',
          'blue',
          'light-blue',
          'cyan',
          'teal',
          'green',
          'light-green',
          'lime',
          'yellow',
          'amber',
          'orange',
          'deep-orange',
          'brown',
          'blue-grey',
          'grey',
          'red',
          'pink',
          'purple',
          'deep-purple',
          'indigo',
          'blue',
          'light-blue',
          'cyan',
          'teal',
          'green',
          'light-green',
          'lime',
          'yellow',
          'amber',
          'orange',
          'deep-orange',
          'brown',
          'blue-grey',
          'grey'
        ]
      }
    }
  }
</script>

<style lang="stylus">
  .custom-ripple
    user-select: none
</style>
