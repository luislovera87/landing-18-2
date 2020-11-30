<template>
  <v-row
    id="section-five-container"
    no-gutters
    class="py-lg-15 py-15 mx-auto mx-lg-auto mx-md-auto mx-sm-auto"
    justify="center"
    align="start"
  >
    <v-col
      cols="10"
      lg="5"
      md="5"
      sm="10"
      class="left-section-container white--text"
    >
      <v-row align="center" justify="center">
        <div
          class="text-center text-lg-h3 text-md-h3 text-sm-h3 text-h4 font-weight-bold pb-lg-5 pb-md-5 pb-sm-5 pb-5"
        >
          Featured Services
        </div>
        <div
          class="text-center mx-lg-auto mx-md-auto mx-sm-auto mx-auto alternative-text-color py-lg-5 py-md-5 py-sm-5 py-5"
          :style="{ 'max-width': '450px' }"
        >
          Sed ut perspiciatis unde omnis iste natus error sit voluptatem
          accusantium doloremque laudantium.
        </div>
        <div class="d-inline-flex">
          <div>
            <img
              src="../assets/img/landing-184-2.png"
              alt="check-icon"
              width="30"
            />
          </div>
          <v-alert
            color="transparent"
            class="white--text mx-lg-auto mx-md-auto mx-sm-aut0 mx-auto pt-0 pt-lg-0 pt-md-0 pt-sm-0"
            :style="{ 'max-width': '350px' }"
          >
            <div>
              <div class="text-h5 font-weight bold">24/7 Fast Support</div>
              <div class="text-subtitle">
                Suspendisse enim turpis, dictum sed, iaculis a, condimentum nec,
                nisi. Vivamus quis mi. Quisque ut nisi. Maecenas malesuada.
              </div>
            </div>
          </v-alert>
        </div>
        <div class="d-inline-flex">
          <div>
            <img
              src="../assets/img/landing-184-2.png"
              alt="check-icon"
              width="30"
            />
          </div>
          <v-alert
            color="transparent"
            class="white--text mx-lg-auto mx-md-auto mx-sm-aut0 mx-auto pt-0 pt-lg-0 pt-md-0 pt-sm-0"
            :style="{ 'max-width': '350px' }"
          >
            <div class="text-h5 font-weight bold">Free Website Setup</div>
            <div class="text-subtitle">
              Suspendisse enim turpis, dictum sed, iaculis a, condimentum nec,
              nisi. Vivamus quis mi. Quisque ut nisi. Maecenas malesuada.
            </div>
          </v-alert>
        </div>
      </v-row>
    </v-col>
    <v-col cols="11" lg="5" md="5" sm="10">
      <div
        class="right-section-container mx-lg-5 mx-md-5 mx-sm-5 mx-1 pa-lg-10 pa-md-10 pa-sm-10 pa-1 rounded-lg"
      >
        <v-expansion-panels focusable accordion :mandatory="true">
          <v-expansion-panel v-for="(item, i) in panelItems" :key="i">
            <v-expansion-panel-header class="font-weight-bold text-h6 white">
              {{ item.title }}
              <template v-slot:actions>
                <v-icon color="black">add_circle</v-icon>
              </template>
            </v-expansion-panel-header>
            <v-expansion-panel-content class="subtitle-default-text">{{
              item.description
            }}</v-expansion-panel-content>
          </v-expansion-panel>
        </v-expansion-panels>
      </div>
    </v-col>
  </v-row>
</template>

<script>
export default {
  data() {
    return {
      panelItems: [
        {
          title: "Sed ut perspiciatis unde omnis?",
          description:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore sint occaecat cupidatat non proident dolore magna aliqua.",
        },
        {
          title: "Veritatis et quasi architecto beatae?",
          description:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore sint occaecat cupidatat non proident dolore magna aliqua.",
        },
        {
          title: "Nemo enim ipsam voluptatem voluptas?",
          description:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore sint occaecat cupidatat non proident dolore magna aliqua.",
        },
        {
          title: "Fugiat quo voluptas nulla pariatur?",
          description:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore sint occaecat cupidatat non proident dolore magna aliqua.",
        },
        {
          title: "Voluptate velit esse cillum dolot?",
          description:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore sint occaecat cupidatat non proident dolore magna aliqua.",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
#section-five-container {
  background-color: #13151c;
}

.right-section-container {
  border-top: 10px solid;
  border-top-color: #68d585 !important;
  background-color: #ffffff;
}

.alternative-text-color {
  font-family: "DM Sans", Helvetica, Arial, Lucida, sans-serif;
  font-size: 18px;
  line-height: 1.8em;
  color: "#ffffffb3!important";
}
</style>