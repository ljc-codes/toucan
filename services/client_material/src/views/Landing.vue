<template>
<div>

  <div class="wrapper">
    <parallax class="section header-filter" :style="headerStyle">
        <v-container class="grey lighten-5">
    <v-row no-gutters>
      <v-col lg="7">
        <v-card
          img="@/assets/img/navbar.jpg"
          flat
          tile
        >
          <h1 class="title">artemis</h1>
            <h4>
              Find bargain companies, dive into fundamentals, share your investment theses with the community.
            </h4>
            <br />
            <md-button
              href="#/signup"
              class="md-rose md-lg"
              ><i class="fas fa-user-plus"></i>Sign up today</md-button
            >
        </v-card>
      </v-col>
      <v-col lg="5">
        <br><br>
        <v-card
          class="pa-2"
          
          flat
          tile
        >
          <WelcomeGraph></WelcomeGraph>
          
        </v-card>
      </v-col>
    </v-row>
  </v-container>
      <div class="container">
        



        <div class="md-layout">
          <div
            class="md-layout-item md-size-50 md-small-size-70 md-xsmall-size-100"
          >
          </div>
        </div>
      </div>
    </parallax>
    <div class="main main-raised">
      <div class="section">
        <div class="container">
          <div class="md-layout">

            <v-row no-gutters> 
              <v-col>
                <img src="@/assets/img/svg/community.svg" width="800" height="200">
              </v-col>
              <v-col>
                <h2 class="title text-center">Let's talk community</h2>
                <h5 class="description">
                  This is the paragraph where you can write more details about
                  your product. Keep you user engaged by providing meaningful
                  information. Remember that by this time, the user is curious,
                  otherwise he wouldn't scroll to get here. Add a button if you
                  want the user to see more.
                </h5>
              </v-col>
            </v-row>
          </div>
          <div class="features text-center">
            <div class="md-layout">
              <div class="md-layout-item md-medium-size-33 md-small-size-100">
                <div class="info">
                  <div class="icon icon-info">
                    <v-icon large left>
                        mdi-binoculars
                    </v-icon>
                  </div>
                  <h4 class="info-title">Explore</h4>
                  <p>
                  </p>
                </div>
              </div>
              <div class="md-layout-item md-medium-size-33 md-small-size-100">
                <div class="info">
                  <div class="icon icon-success">
                     <v-icon large left>
                        mdi-sword
                    </v-icon>
                  </div>
                  <h4 class="info-title">Analyze</h4>
                  <p>
                  </p>
                </div>
              </div>
              <div class="md-layout-item md-medium-size-33 md-small-size-100">
                <div class="info">
                  <div class="icon icon-danger">
                    <v-icon large left>
                        mdi-message-processing
                    </v-icon>
                  </div>
                  <h4 class="info-title">Share </h4>
                  <p>
                  </p>
                </div>
              </div>
            </div>
            <div class="md-layout">
            <br>

            <v-row no-gutters> 
              <v-col>
                <h2 class="title text-center">Let's talk data</h2>
                <h5 class="description">
                  This is the paragraph where you can write more details about
                  your product. Keep you user engaged by providing meaningful
                  information. Remember that by this time, the user is curious,
                  otherwise he wouldn't scroll to get here. Add a button if you
                  want the user to see more.
                </h5>  
              </v-col>
              <v-col>
                <img src="@/assets/img/svg/data.svg" width="800" height="200">
              </v-col>
            </v-row>
          </div>
          </div>
        </div>
      </div>
      </div>
      <br>
        
   

  </div>
</div>
   
</template>

<script>
import  WelcomeGraph  from "@/components/graphs/WelcomeGraph.vue";
export default {
  bodyClass: "landing-page",
  props: {
    header: {
      type: String,
      default: require("@/assets/img/background_welcome.jpg")
    }
  },
  components: { WelcomeGraph },
  data() {
    return {
      name: null,
      email: null,
      message: null,
      show_search: false
    };
  },
  computed: {
    headerStyle() {
      return {
        backgroundImage: `url(${this.header})`
      };
    }
  }
};
</script>

<style lang="scss" scoped>
.md-card-actions.text-center {
  display: flex;
  justify-content: center !important;
}
.contact-form {
  margin-top: 30px;
}

.md-has-textarea + .md-layout {
  margin-top: 15px;
}

body{
  font-family: 'PT Sans', sans-serif;
  background-color: #6f92e8;
}
</style>

