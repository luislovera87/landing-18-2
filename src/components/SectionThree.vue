<template>
  <v-row no-gutters>
    <v-col cols="12" lg="12" class="py-lg-15 py-md-8 py-sm-15 py-5">
      <v-row no-gutters justify="center" align="center">
        <v-col cols="9" lg="12">
          <div
            class="text-center text-lg-h3 text-md-h3 text-sm-h3 text-h4 font-weight-bold pb-lg-5 pb-md-5 pb-sm-5 pb-5"
          >
            Featured Services
          </div>
          <div
            class="text-center subtitle-default-text mx-lg-auto mx-md-auto mx-sm-auto mx-auto"
            :style="{ 'max-width': '500px' }"
          >
            Sed ut perspiciatis unde omnis iste natus error sit voluptatem
            accusantium doloremque laudantium.
          </div>
        </v-col>
      </v-row>
    </v-col>
    <v-col cols="12" lg="12">
      <v-row no-gutters align="center" justify="center">
        <v-hover v-slot="{ hover }">
          <v-col
            cols="12"
            lg="3"
            md="3"
            sm="3"
            class="mx-lg-5 mx-md-3 mx-sm-3 mx-3 text-center"
            :class="hover ? 'image-hover-effect' : ''"
          >
            <img
              src="../assets/img/landing-183-1.jpg"
              alt="Img-1"
              class="rounded-lg"
              :style="{ 'max-width': '100%', height: 'auto' }"
            />
            <div class="image-title-text text-h5 font-weight-bold text-center">
              Web Site Design
            </div>
            <div
              class="subtitle-default-text text-overline text-center font-weight-bold"
            >
              READ MORE
            </div>
          </v-col>
        </v-hover>
        <v-hover v-slot="{ hover }">
          <v-col
            cols="12"
            lg="3"
            md="3"
            sm="3"
            class="mx-lg-5 mx-md-3 mx-sm-3 mx-3 text-center"
            :class="hover ? 'image-hover-effect' : ''"
          >
            <img
              src="../assets/img/landing-183-2.jpg"
              alt="Img-1"
              class="rounded-lg"
              :style="{ 'max-width': '100%', height: 'auto' }"
            />
            <div class="image-title-text text-h5 font-weight-bold text-center">
              Google Advertise
            </div>
            <div
              class="subtitle-default-text text-overline text-center font-weight-bold"
            >
              READ MORE
            </div>
          </v-col>
        </v-hover>
        <v-hover v-slot="{ hover }">
          <v-col
            cols="12"
            lg="3"
            md="3"
            sm="3"
            class="mx-lg-5 mx-md-3 mx-sm-3 mx-3 text-center"
            :class="hover ? 'image-hover-effect' : ''"
          >
            <img
              src="../assets/img/landing-183-3.jpg"
              alt="Img-1"
              class="rounded-lg"
              :style="{ 'max-width': '100%', height: 'auto' }"
            />
            <div class="image-title-text text-h5 font-weight-bold text-center">
              Other Services
            </div>
            <div
              class="subtitle-default-text text-overline text-center font-weight-bold"
            >
              READ MORE
            </div>
          </v-col>
        </v-hover>
      </v-row>
    </v-col>
  </v-row>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.image-hover-effect {
  cursor: pointer;
  transition: color 300ms ease 0ms, filter 300ms ease 0ms;
  opacity: 1;
  &:hover {
    filter: opacity(60%);
    .image-title-text {
      color: #68d585 !important;
    }
  }
}
</style>