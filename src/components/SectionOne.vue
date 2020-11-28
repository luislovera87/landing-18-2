<template>
  <v-row no-gutters>
    <v-col cols="12" class="landing-section-0 with-background">
      <v-row>
        <v-col
          cols="12"
          class="text-overline text-center your-content-text pt-lg-0 pt-0"
          :style="{ color: '#68D585!important' }"
        >
          YOUR CONTENT GOES HERE
        </v-col>
        <v-col
          cols="12"
          class="text-lg-h2 text-md-h3 text-sm-h4 text-h3 landing-title-0 mt-lg-0 mt-lg-0 white--text mx-lg-auto mx-md-auto mx-sm-auto mx-auto text-center"
        >
          Clean landing page theme for divi builder
        </v-col>
        <v-col cols="12" lg="12">
          <v-row justify="center">
            <v-col cols="9" lg="7" class="d-inline-flex white rounded-lg">
              <v-row justify="center" align="center">
                <v-col cols="12" lg="4">
                  <v-text-field
                    label="Solo"
                    placeholder="First Name"
                    solo
                    full-width
                    height="100%"
                    hide-details="auto"
                  ></v-text-field>
                </v-col>
                <v-col cols="12" lg="4">
                  <v-text-field
                    label="Solo"
                    placeholder="Last Name"
                    solo
                    full-width
                    height="100%"
                    hide-details="auto"
                  ></v-text-field
                ></v-col>
                <v-col cols="12" lg="3">
                  <v-hover v-slot="{ hover }"
                    ><v-btn
                      class="subscribe-button"
                      :color="hover ? 'success' : 'accent'"
                      width="100%"
                      height="56px"
                    >
                      Subscribe
                    </v-btn></v-hover
                  ></v-col
                >
              </v-row>
            </v-col>
          </v-row>
        </v-col>
        <v-col
          cols="12"
          class="white--text text-overline text-center your-content-text pt-lg-5 pt-5"
        >
          <v-icon :v-text="'play-circle-outline'"></v-icon>
          YOUR VIDEO CONTENT GOES HERE
        </v-col>
      </v-row>
    </v-col>
  </v-row>
</template>

<script>
export default {
  data() {
    return {
      buttonColor: "accent",
    };
  },
  methods: {
    onActiveButton() {
      this.buttonColor = "success";
    },
    onDefaultButton() {
      this.buttonColor = "accent";
    },
  },
};
</script>

<style lang="scss" scoped>
.landing-section-0 {
  padding: 30vh 0 !important;
  &.with-background {
    background-image: linear-gradient(
        180deg,
        rgba(8, 12, 22, 0.81) 0%,
        rgba(8, 12, 22, 0.81) 100%
      ),
      url(../assets/img/landing-184-1.jpg) !important;
    background-size: cover;
    background-position: 50%;
    background-repeat: no-repeat;
    height: 850px;
  }
  .your-content-text {
    font-family: "DM Sans", Helvetica, Arial, Lucida, sans-serif !important;
    font-weight: 700;
    text-transform: uppercase;
    font-size: 13px;
    letter-spacing: 1px;
    line-height: 1em;
  }

  .landing-title-0 {
    max-width: 780px;
    font-family: "DM Sans", Helvetica, Arial, Lucida, sans-serif !important;
    font-weight: 700;
    color: #ffffff !important;
    letter-spacing: -2px;
    line-height: 1.3em;
  }

  .subscribe-button {
    transition: background-color 0.3s ease-in-out;
  }

  .subscribe-button {
    transition: background-color 0.3s ease-in-out;
  }
}

@media only screen and (max-width: 767px) {
  .landing-section-0 {
    padding: 10vh 0 !important;
  }
  .landing-section-0.with-background {
    height: 700px;
    margin-bottom: 100px;
  }
}
</style>