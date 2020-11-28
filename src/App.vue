<template>
  <v-app>
    <v-main>
      <v-container fluid class="pa-0 pa-lg-0">
        <SectionOne />
        <SectionTwo />
        <v-row>
          <v-col cols="12" lg="12">
            <v-divider></v-divider>
          </v-col>
        </v-row>
        <SectionThree />
      </v-container>
    </v-main>
  </v-app>
</template>

<script>
import SectionOne from "./components/SectionOne.vue";
import SectionTwo from "./components/SectionTwo.vue";
import SectionThree from "./components/SectionThree.vue";

export default {
  name: "App",

  components: {
    SectionOne,
    SectionTwo,
    SectionThree,
  },

  data: () => ({
    //
  }),
};
</script>

<style lang="scss">
html,
body {
  overflow: hidden;
  font-family: Open Sans, Arial, sans-serif;
  font-size: 14px;
  color: #666;
  background-color: #fff;
  line-height: 1.7em;
  font-weight: 500;
  -webkit-font-smoothing: antialiased;
}

body,
input,
textarea,
select {
  font-family: "Lato", Helvetica, Arial, Lucida, sans-serif;
}
</style>
