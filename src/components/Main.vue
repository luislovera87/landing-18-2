<template>
  <div>
    <div id="background-section">
      <div style="padding-top: 30vh" class="box-one container-fluid px-0">
        <div class="custom-content-label text-center font-weight-bold">
          YOUR CONTENT GOES HERE
        </div>
        <div class="d-flex justify-center">
          <div style="width: 50vw; padding-top: 15px">
            <h1>Clean landing page theme for divi builder</h1>
          </div>
        </div>
      </div>
    </div>
    <div id="metrics-section">
      <div class="row box-one text-center align-center justify-center">
        <div class="percent-box col-md-3 col-12">
          <div class="percent">
            <p>
              <span class="percent-value">87</span>
              <span class="percent-sign">+</span>
            </p>
          </div>
          <div class="percent-description default-text-medium">
            Lorem ipsum dolor sit amet consec tetur elit.
          </div>
        </div>
        <div class="percent-box col-md-3 col-12">
          <div class="percent">
            <p>
              <span class="percent-value">49</span>
              <span class="percent-sign"></span>
            </p>
          </div>
          <div class="percent-description default-text-medium">
            Lorem ipsum dolor sit amet consec tetur elit.
          </div>
        </div>
        <div class="percent-box col-md-3 col-12">
          <div class="percent">
            <p>
              <span class="percent-value">382</span>
              <span class="percent-sign"></span>
            </p>
          </div>
          <div class="percent-description default-text-medium">
            Lorem ipsum dolor sit amet consec tetur elit.
          </div>
        </div>
      </div>
    </div>
    <hr />
    <div id="featured-services-section">
      <div
        class="row box-one text-center align-center justify-center mt-md-10 mt-10 mx-sm-5"
      >
        <h1>Featured Services</h1>
        <div class="d-flex col-12 col-md-12 align-center justify-center">
          <div class="default-text-medium" style="max-width: 575px">
            Sed ut perspiciatis unde omnis iste natus error sit voluptatem
            accusantium doloremque laudantium.
          </div>
        </div>
      </div>
      <div
        class="row box-two text-center align-center justify-center mt-md-10 mt-10"
      >
        <div class="col-12 col-lg-3 rounded-lg featured-service-box">
          <img
            src="../assets/img/landing-183-1.jpg"
            alt="landing-183-1.jpg"
            width="350"
          />
          <div class="featured-service-box-img-description">
            <h2>Web Site Design</h2>
            <small>READ MORE</small>
          </div>
        </div>
        <div class="col-12 col-lg-3 rounded-lg featured-service-box">
          <img
            src="../assets/img/landing-183-2.jpg"
            alt="landing-183-2.jpg"
            width="350"
          />
          <div class="featured-service-box-img-description">
            <h2>Web Site Design</h2>
            <small>READ MORE</small>
          </div>
        </div>
        <div class="col-12 col-lg-3 rounded-lg featured-service-box">
          <img
            src="../assets/img/landing-183-3.jpg"
            alt="landing-183-3.jpg"
            width="350"
          />
          <div class="featured-service-box-img-description">
            <h2>Web Site Design</h2>
            <small>READ MORE</small>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Main',
  data() {
    return {
      items: [
        {
          text: 'Website Design',
          img:
            'https://149448400.v2.pressablecdn.com/wp-content/uploads/2020/10/landing-183-1.jpg',
        },
        {
          text: 'Google Advertise',
          img:
            'https://149448400.v2.pressablecdn.com/wp-content/uploads/2020/10/landing-183-2.jpg',
        },
        {
          text: 'Other Services',
          img:
            'https://149448400.v2.pressablecdn.com/wp-content/uploads/2020/10/landing-183-3.jpg',
        },
      ],
      transparent: 'rgba(255, 255, 255, 0)',
    };
  },
};
</script>

<style lang="scss" scoped>
#background-section {
  .box-one {
    .custom-content-label {
      color: #68d585 !important;
      font-family: "DM Sans", Helvetica, Arial, Lucida, sans-serif;
      font-weight: 700;
      text-transform: uppercase;
      font-size: 13px;
      letter-spacing: 1px;
      line-height: 1em;
    }
    h1 {
      font-family: "DM Sans", Helvetica, Arial, Lucida, sans-serif;
      font-weight: 700;
      font-size: 60px;
      color: #ffffff !important;
      letter-spacing: -2px;
      line-height: 1.3em;
      text-align: center;
    }
  }

  background-image: linear-gradient(
      180deg,
      rgba(8, 12, 22, 0.81) 0%,
      rgba(8, 12, 22, 0.81) 100%
    ),
    url(../assets/img/landing-184-1.jpg) !important;
  background-size: cover;
  background-position: 50%;
  background-repeat: no-repeat;
  height: 800px;
}

#metrics-section {
  .box-one {
    font-family: "DM Sans", Helvetica, Arial, Lucida, sans-serif;
    font-size: 18px;
    line-height: 1.8em;
    margin-top: -25px !important;
    padding-top: 90px;
    padding-bottom: 84px;
  }
}

#featured-services-section {
  h1 {
    font-family: "DM Sans", Helvetica, Arial, Lucida, sans-serif;
    font-weight: 700;
    font-size: 48px;
    color: #161c2d !important;
    letter-spacing: -2px;
    text-align: center;
  }
  .box-two {
    .featured-service-box {
      img {
        cursor: pointer;
        transition: color 300ms ease 0ms, filter 300ms ease 0ms;
        opacity: 1;
        &:hover {
          filter: opacity(60%);
          & + .featured-service-box-img-description {
            color: #68d585 !important;
          }
        }
      }
      .featured-service-box-img-description {
        small {
          font-family: "DM Sans", Helvetica, Arial, Lucida, sans-serif;
          font-weight: 700;
          font-size: 12px;
          color: rgba(22, 28, 45, 0.7) !important;
          letter-spacing: 1px;
          line-height: 1.8em;
        }
      }
    }
  }
}
</style>
