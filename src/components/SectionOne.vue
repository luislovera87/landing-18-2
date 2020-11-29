<template>
  <v-row no-gutters>
    <v-col cols="12" lg="12" class="landing-section-0 with-background">
      <v-row no-gutters>
        <v-col
          cols="12"
          class="text-overline text-center your-content-text pt-lg-0 pt-0"
          :style="{ color: '#68D585!important' }"
        >
          YOUR CONTENT GOES HERE
        </v-col>
        <v-col
          cols="12"
          lg="6"
          md="6"
          sm="6"
          class="text-lg-h2 text-md-h3 text-sm-h3 text-h3 landing-title-0 mt-lg-0 mt-lg-0 white--text mx-lg-auto mx-md-auto mx-sm-auto mx-auto text-center py-lg-5 py-md-5 py-sm-5 py-5"
        >
          Clean landing page theme for divi builder
        </v-col>
        <v-col cols="12" lg="12">
          <v-row no-gutters justify="center">
            <v-col cols="9" lg="7" class="d-inline-flex white rounded-lg pa-4">
              <v-row no-gutters justify="center" align="center">
                <v-col cols="12" lg="4" class="py-2">
                  <v-text-field
                    label="Solo"
                    placeholder="First Name"
                    solo
                    full-width
                    height="100%"
                    hide-details="auto"
                  ></v-text-field>
                </v-col>
                <v-col cols="12" lg="4" class="py-2">
                  <v-text-field
                    label="Solo"
                    placeholder="Last Name"
                    solo
                    full-width
                    height="100%"
                    hide-details="auto"
                  ></v-text-field
                ></v-col>
                <v-col cols="12" lg="3" class="py-2">
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
          <v-row no-gutters align="center" justify="center">
            <v-hover v-slot="{ hover }">
              <v-col
                lg="3"
                md="3"
                sm="12"
                cols="12"
                class="video-content-text"
                :class="{ 'transform-zoom': hover }"
              >
                <v-icon class="white--text">play_circle_outline</v-icon>
                YOUR VIDEO CONTENT GOES HERE
              </v-col>
            </v-hover>
          </v-row>
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

.video-content-text.transform-zoom {
  cursor: pointer;
  transform: scaleX(1.1) scaleY(1.1) !important;
  transition: 0.3s transform ease-in-out;
}

.video-content-text:not(.transform-zoom) {
  transition: 0.3s transform ease-in-out;
}
</style>