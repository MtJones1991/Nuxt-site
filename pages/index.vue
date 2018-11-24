<template>

<div>

 <v-parallax
    class="paraImg elevation-21"
    src="https://i.imgur.com/lpdgiTV.jpg" 
  >
      <v-layout align-center justify-center column fill-height>
          <Logo/>
      </v-layout>
  </v-parallax>

        <v-layout align-center justify-center column fill-height wrap>
            <h1 data-aos="fade" data-aos-duration="2000" data-aos-mirror="true" wrap  data-aos-easing="ease-in-out" class="mt-5 titleTop text-xs-center">Nuxt and Veutify</h1>
        </v-layout>

        <v-layout align-center justify-center column fill-height wrap>
            <p data-aos="fade" data-aos-duration="2000" data-aos-mirror="true" wrap data-aos-easing="ease-in-out" class="mb-5 text-xs-center">This website showcase the use of Veutify, Nuxt and AOS</p>
        </v-layout>

        <v-spacer class="mt-5"></v-spacer>

    <v-layout align-center justify-space-around row fill-height wrap>
      <v-card  data-aos="fade-right" data-aos-duration="1500" data-aos-mirror="true" data-aos-anchor-placement="top-center" class="cards text-xs-center">
        <v-img
          class="cardImg"
          src="https://picsum.photos/610/300?image=867"
          height="150px"
        >
        </v-img>
        
        <v-card-title primary-title>
          <div>
            <div class="headline text-xs-center">Fluid  & material design</div>
            <span class="grey--text text-xs-center">Using the Vuetify framework</span>
          </div>
        </v-card-title>
      </v-card>

      <v-card  data-aos="fade-down" data-aos-duration="1900" data-aos-mirror="true" data-aos-anchor-placement="top-center" class="cards text-xs-center">
        <v-img
          class="cardImg elevation-13"
          src="https://picsum.photos/710/300/?image=877"
          height="150px"
        >
        </v-img>

        <v-card-title primary-title>
          <div>
            <div class="headline text-xs-center">Built with Vue & Nuxt.js</div>
            <span class="grey--text text-xs-center">1,000 miles of wonder</span>
          </div>
        </v-card-title>
      </v-card>

      <v-card data-aos="fade-left" data-aos-duration="2100" data-aos-mirror="true" data-aos-anchor-placement="top-center" class="cards text-xs-center">
        <v-img
          class="cardImg elevation-13"
          src="https://picsum.photos/410/300?image=914"
          height="150px"
        >
        </v-img>

        <v-card-title primary-title>
          <div>
            <div class="headline text-xs-center">Top western road trips</div>
            <span class="grey--text text-xs-center">1,000 miles of wonder</span>
          </div>
        </v-card-title>
      </v-card>
      
  </v-layout>


   <v-parallax
    class="paraImg elevation-21 mb-5 mt-5"
    src="https://picsum.photos/1080/720?image=171" 
  >
      <v-layout align-center justify-center column fill-height>
        <h4 
        class="display-1 pt-5 mt-5"
        color="white"
        data-aos="zoom-in" data-aos-duration="2100" data-aos-mirror="true"
        ><nuxt-link class="inspire" to="/inspire">Inspire</nuxt-link></h4>
      </v-layout>
  </v-parallax>

  <BottomNav/>
  
  </div>
  
  
</template>

<script>
import Logo from '~/components/Logo.vue'
import VuetifyLogo from '~/components/VuetifyLogo.vue'
import BottomNav from '~/components/BottomNav.vue'
export default {
  components: {
    Logo,
    VuetifyLogo,
    BottomNav
  },
    data: () => ({
      show: false
    })
}
</script>

<style>
element.style {
     height: 500px;
}
.titleTop {
  color: tomato;
}
.v-parallax {
  height: 600px !important;
  width: 100%;
  margin-top: 25px;
}
.inspire {
  color: whitesmoke;
  margin-top: 10px;
  text-decoration: none;
  font-family: 'Montserrat' !important;
}
.headlineTitle {
  /* border-radius: 50%; */
  background-color: brown;
}
.cards {
  border-radius: 100%;
  background-color: transparent !important;
  border: none !important;
}
.v-card {
  box-shadow: none !important;
  text-align: center;
}
.cardImg {
  width: 150px;
  display: inline-block;
  border-radius: 100%;
}
.headline {
    font-family: 'Montserrat' !important;
}
</style>