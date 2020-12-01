<template>
  <v-app>
    <v-main>
      <v-container
        fluid
        class="pa-0 pa-lg-0"
        :style="{ 'overflow-y': 'hidden' }"
      >
        <SectionOne />
        <SectionTwo />
        <DefaultDivider />
        <SectionThree />
        <SectionFour />
        <SectionFive />
      </v-container>
    </v-main>
  </v-app>
</template>

<script>
import SectionOne from "./components/SectionOne.vue";
import SectionTwo from "./components/SectionTwo.vue";
import SectionThree from "./components/SectionThree.vue";
import SectionFour from './components/SectionFour.vue';
import SectionFive from './components/SectionFive';
import DefaultDivider from "./components/DefaultDivider.vue";

export default {
  name: "App",

  components: {
    SectionOne,
    SectionTwo,
    SectionThree,
    SectionFour,
    SectionFive,
    DefaultDivider,
  },

  data: () => ({
    //
  }),
};
</script>

<style lang="scss">

html,
body {
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

.subtitle-default-text {
  color: rgba(22, 28, 45, 0.7) !important;
  font-family: "DM Sans", Helvetica, Arial, Lucida, sans-serif;
  font-size: 18px;
  line-height: 1.8em;
  font-weight: 600;
}
</style>
