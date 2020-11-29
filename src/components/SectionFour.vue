<template>
  <v-row
    no-gutters
    justify="center"
    align="start"
    class="py-lg-15 py-15 section-four-container"
  >
    <v-col cols="12" lg="5" md="6" sm="12" class="mx-auto mx-lg-auto">
      <v-row no-gutters justify="center" align="center">
        <v-col cols="12" lg="12" md="9" sm="9">
          <div
            class="text-center text-lg-h3 text-md-h3 text-sm-h3 text-h4 font-weight-bold pb-lg-5 pb-md-5 pb-sm-5 pb-5"
          >
            Archit beatae vitae ticta explicabo.
          </div>
          <div
            class="text-center subtitle-default-text mx-lg-auto mx-md-auto mx-sm-auto mx-auto"
            :style="{ 'max-width': '500px' }"
          >
            Sed ut perspiciatis unde omnis iste natus error sit voluptatem
            accusantium.
          </div>
        </v-col>
        <img
          src="../assets/img/landing-181-1.jpg"
          alt="Img-1"
          class="rounded-lg mx-lg-auto py-lg-5 py-md-5 py-sm-5 py-5"
          width="auto"
          height="auto"
        />
      </v-row>
    </v-col>
    <v-col cols="12" lg="5" md="6" sm="12" class="mx-auto mx-lg-auto">
      <v-row no-gutters justify="center" align="center">
        <img
          src="../assets/img/landing-181-2.jpg"
          alt="Img-1"
          class="rounded-lg mx-lg-auto py-lg-5 py-md-5 py-sm-5 py-5"
          width="auto"
          height="auto"
        />
      </v-row>
    </v-col>
  </v-row>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.section-four-container {
  background: linear-gradient(180deg, #f4f7fa 65%, #ffffff 0%) !important;
}
</style>