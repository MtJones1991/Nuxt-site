<template>

    <section>
        <v-layout
          column
          wrap
          class="my-5"
          align-center
        >
          <v-flex xs12 sm4 class="my-3">
            <div class="text-xs-center">
              <h2 class="headline">The best way to start developing</h2>
              <span class="subheading">
                Cras facilisis mi vitae nunc 
              </span>
            </div>
          </v-flex>
          <v-flex xs12>
            <v-container grid-list-xl>
              <v-layout row wrap align-center>
                <v-flex xs12 md4>


                  <v-card class="elevation-0 transparent" data-aos="fade" data-aos-duration="1500" >
                    <v-card-text class="text-xs-center">
                      <v-icon x-large class="orange--text text--lighten-1">fas fa-paint-brush</v-icon>
                    </v-card-text>
                    <v-card-title primary-title class="layout justify-center">
                      <div class="headline text-xs-center">Material Design</div>
                    </v-card-title>
                    <v-card-text>
                      Cras facilisis mi vitae nunc lobortis pharetra. Nulla volutpat tincidunt ornare. 
                      Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. 
                      Nullam in aliquet odio. Aliquam eu est vitae tellus bibendum tincidunt. Suspendisse potenti. 
                    </v-card-text>
                  </v-card>


                </v-flex>
                <v-flex xs12 md4>


                  <v-card class="elevation-0 transparent" data-aos="fade" data-aos-duration="1500" >
                    <v-card-text class="text-xs-center">
                      <v-icon x-large class="orange--text text--lighten-1">fas fa-camera</v-icon>
                    </v-card-text>
                    <v-card-title primary-title class="layout justify-center">
                      <div class="headline">Fast development</div>
                    </v-card-title>
                    <v-card-text>
                      Cras facilisis mi vitae nunc lobortis pharetra. Nulla volutpat tincidunt ornare. 
                      Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. 
                      Nullam in aliquet odio. Aliquam eu est vitae tellus bibendum tincidunt. Suspendisse potenti. 
                    </v-card-text>
                  </v-card>


                </v-flex>
                <v-flex xs12 md4>


                  <v-card class="elevation-0 transparent" data-aos="fade" data-aos-duration="1500" >
                    <v-card-text class="text-xs-center">
                      <v-icon x-large class="orange--text text--lighten-1">fab fa-accusoft</v-icon>
                    </v-card-text>
                    <v-card-title primary-title class="layout justify-center">
                      <div class="headline text-xs-center">Completely Open Sourced</div>
                    </v-card-title>
                    <v-card-text>
                      Cras facilisis mi vitae nunc lobortis pharetra. Nulla volutpat tincidunt ornare. 
                      Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. 
                      Nullam in aliquet odio. Aliquam eu est vitae tellus bibendum tincidunt. Suspendisse potenti. 
                    </v-card-text>
                  </v-card>


                </v-flex>
              </v-layout>
            </v-container>
          </v-flex>
        </v-layout>
      </section>

</template>

<script>
  export default {

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

.links {
  color: whitesmoke;
}

.text, .bottomText {
    font-family: 'Montserrat' !important;
}

.navCard {
  width: 100%;
}

</style>