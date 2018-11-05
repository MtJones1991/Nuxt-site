<template>
  <div>
      <v-layout align-center justify-center column fill-height>
      <h1 class="mt-3 mb-5">Home</h1>
      <v-btn color="warning" class="mt-3 mb-5">
        <nuxt-link to="/">Home</nuxt-link>
      </v-btn>
        <!-- <Logo/> -->
      </v-layout>

  <v-item-group>
    <v-container grid-list-md>
      <v-layout wrap>
        <v-flex
          v-for="n in 3"
          :key="n"
          xs12
          md4
        >
          <v-item class="cardA">
            <v-card
              slot-scope="{ active, toggle }"
              class="d-flex align-center"
              dark
              height="265"
            >
                      <v-img
          class="cardImg"
          src="https://picsum.photos/610/300?image=867"
          height="265px"
        >
        </v-img>
            </v-card>
          </v-item>
        </v-flex>
      </v-layout>
    </v-container>
  </v-item-group>
  <BottomNav/>
  </div>
</template>

<script>
import BottomNav from '~/components/BottomNav.vue'

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
