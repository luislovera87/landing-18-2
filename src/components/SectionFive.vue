<template>
  <v-row
    id="section-five-container"
    no-gutters
    class="py-lg-15 py-15"
    justify="center"
    align="center"
  >
    <v-col lg="5" md="12" sm="12" cols="12" class="white--text">
      <v-row no-gutters justify="start" align="center">
        <v-col
          cols="9"
          md="10"
          sm="9"
          lg="12"
          class="pb-lg-5 pb-md-5 pb-sm-5 pb-5 pl-lg-0 pl-md-15 pl-sm-15 pl-15"
        >
          <v-row justify="start" align="center">
            <v-col
              cols="12"
              lg="12"
              md="12"
              sm="12"
              class="text-lg-h3 text-md-h3 text-sm-h3 text-h4 font-weight-bold"
              :style="{ 'max-width': '500px' }"
            >
              Exercita tion ullam corpor suscit.
            </v-col>
            <v-col
              cols="12"
              lg="12"
              md="12"
              sm="12"
              class="subtitle-default-text white--text"
              :style="{ 'max-width': '500px' }"
            >
              Sed ut perspiciatis unde omnis iste natus error sit voluptatem
              accusantium.
            </v-col>
            <v-col
              cols="12"
              lg="12"
              md="12"
              sm="12"
              :style="{ 'max-width': '500px' }"
            >
              <v-row>
                <div class="d-inline-flex">
                  <div>
                    <img
                      src="../assets/img/landing-184-2.png"
                      alt="check-icon"
                      width="30"
                      height="30"
                    />
                  </div>
                  <div class="check-description-container text-left">
                    <div class="font-weight-bold text-h6">
                      24/7 Fast Support
                    </div>
                    <div
                      class="subtitle-default-text alternative-text-color text-body-1"
                      :style="{ 'max-width': '300px' }"
                    >
                      Esse quam nihil molestiae conse vel illum eum fugiat
                      voluptas nulla exceurs pariatur.
                    </div>
                  </div>
                </div>
              </v-row>
              <v-row>
                <div class="d-inline-flex">
                  <div>
                    <img
                      src="../assets/img/landing-184-2.png"
                      alt="check-icon"
                      width="30"
                      height="30"
                    />
                  </div>
                  <div class="check-description-container text-left">
                    <div class="font-weight-bold text-h6">
                      Free Website Setup
                    </div>
                    <div
                      class="subtitle-default-text alternative-text-color text-body-1"
                      :style="{ 'max-width': '300px' }"
                    >
                      Esse quam nihil molestiae conse vel illum eum fugiat
                      voluptas nulla exceurs pariatur.
                    </div>
                  </div>
                </div>
              </v-row>
            </v-col>
          </v-row>
        </v-col>
      </v-row>
    </v-col>
    <v-col lg="5" md="12" sm="12" cols="12" class="pl-lg-15 pl-md-15 pl-sm-15 pl-8">
      <v-row align="center" justify="start">
        <v-col
          lg="12"
          md="8"
          sm="11"
          cols="11"
          class="right-section-container rounded-lg"
        >
          <v-expansion-panels focusable accordion :mandatory="true">
            <v-expansion-panel v-for="(item, i) in panelItems" :key="i">
              <v-expansion-panel-header class="font-weight-bold text-h6 white">
                {{ item.title }}
                <template v-slot:actions>
                  <v-icon color="black">add_circle</v-icon>
                </template>
              </v-expansion-panel-header>
              <v-expansion-panel-content
                class="subtitle-default-text text-body-1"
                >{{ item.description }}</v-expansion-panel-content
              >
            </v-expansion-panel>
          </v-expansion-panels>
        </v-col>
      </v-row>
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
  color: #ffffffb3 !important;
}

.check-description-container {
  padding: 0 20px 20px 20px;
}
</style>