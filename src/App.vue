<template>
  <v-app>
    <v-main>
      <Main />
    </v-main>
  </v-app>
</template>

<script>
import Main from "./components/Main";

export default {
  name: "App",

  components: {
    Main,
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

.default-text-medium {
  font-family: "DM Sans", Helvetica, Arial, Lucida, sans-serif;
  font-size: 18px;
  line-height: 1.8em;
  color: rgba(22, 28, 45, 0.7) !important;
}

.percent-box {
  .percent {
    margin: auto;
    height: 72px;
    p {
      font-family: "DM Sans", Helvetica, Arial, Lucida, sans-serif;
      font-weight: 700;
      font-size: 50px;
      color: #161c2d !important;
      letter-spacing: -2px;
      line-height: 42px;
      text-align: center;
    }
  }
  .percent-description {
    margin: auto;
    margin-bottom: 30px;
    max-width: 275px;
  }
}
</style>
