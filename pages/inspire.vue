<template>
<div>
    <v-layout align-center justify-center column fill-height>
        <v-layout align-center justify-center column fill-height class="pb-5 mb-5">
            <h4 class="display-1 pt-5 mt-5" color="white" data-aos="zoom-in" data-aos-duration="2100" data-aos-mirror="true">
                <nuxt-link class="inspire" to="/">Home</nuxt-link>
            </h4>
        </v-layout>
        <!-- <Logo/> -->
    </v-layout>

    <BottomNav />
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
.custom-ripple user-select: none .cardA {
    border-radius: 100%;
}
</style>
