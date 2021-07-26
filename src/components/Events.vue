<template>
  <div class="container">
    <div class="header-image"></div>
    <div class="title" data-aos="fade-up" data-aos-delay="100">
      <h2>Events</h2>
    </div>
    <div class="events-container">
      <h3 data-aos="fade-in" data-aos-delay="200">{{ event1 }}</h3>
      <h4 class="date-h4" data-aos="fade-in" data-aos-delay="200">
        <span>date:</span> {{ date }}
      </h4>
      <h4 class="des-h4" data-aos="fade-in" data-aos-delay="200">
        <span>description:</span> SCP-173 is made out of REDACTED. It is super
        fast, but only if you are not looking at it.
      </h4>

      <h3 data-aos="fade-in" data-aos-delay="200">{{ event2 }}</h3>
      <h4 class="date-h4" data-aos="fade-in" data-aos-delay="200">
        <span>date:</span> {{ date }}
      </h4>
      <h4 class="des-h4" data-aos="fade-in" data-aos-delay="200">
        <span>description:</span> Doctor is the cure. He wants to heal you, let
        him to help you.. he.. is.. the cure.
      </h4>
    </div>
  </div>
</template>
<script>
export default {
  name: "Events",
  props: {
    date: String,
    event1: String,
    event2: String,
  },
};
</script>
<style scoped lang="scss">
.container {
  position: relative;
  height: 180vh;
  background-image: linear-gradient(#2c2c50, #2c2c50);
  color: rgb(247, 247, 247);
  z-index: 1;
  h2 {
    padding-top: 300px;
    font-size: 150px;
  }
}
.header-image {
  background-image: url("~@/assets/wave-down.svg");
  background-repeat: no-repeat;
  background-size: contain;
  background-position: top;
  height: 100vh;
  width: 100%;
  top: -10%;
  z-index: -1;
  transform: scaleX(-1);
  position: absolute;
}
.events-container {
  height: 90vh;
  h3 {
    justify-content: center;
    padding-top: 100px;

    line-height: 75px;
    font-size: 70px;
    font-weight: 500;
    .events-date {
      font-size: 30px;
      color: rgb(255, 255, 255);
      font-weight: 400;
    }
    span {
      font-size: 20px;
      font-weight: 300;
    }
  }
  h4 {
    font-size: 18px;
    font-weight: 400;
    span {
      text-transform: uppercase;
      font-weight: 600;
    }
  }
  .date-h4 {
    padding-bottom: 50px;
  }
  .des-h4 {
    padding-bottom: 150px;
  }
}
@media only screen and (min-device-width: 370px) and (max-device-width: 480px) {
  .container {
    height: 220vh;
    h2 {
      font-size: 40px;
    }
  }
  .events-container {
    h3 {
      font-size: 25px;
      padding-bottom: 50px;
      span {
        font-size: 15px;
      }
    }
  }
}
@media only screen and (min-device-width: 200px) and (max-device-width: 360px) {
  .container {
    height: 300vh;
    h2 {
      font-size: 60px;
    }
  }
  .events-container {
    h3 {
      font-size: 25px;
      padding-bottom: 50px;
      span {
        font-size: 15px;
        font-weight: 400;
      }
    }
  }
  .header-image {
    top: 0%;
  }
}
@media screen and (min-device-width: 1200px) and (max-device-width: 1600px) and (-webkit-min-device-pixel-ratio: 1) {
  .header-image {
    top: -5%;
  }
  .container {
    height: 250vh;
  }
}
@media screen and (min-device-width: 2400px) and (max-device-width: 4000px) and (-webkit-min-device-pixel-ratio: 1) {
  .container {
    padding-top: 100px;
    height: 190vh;
    h2 {
      font-size: 240px;
    }
  }
  .events-container {
    height: 90vh;
    h3 {
      font-size: 120px;
      padding-top: 75px;
      .events-date {
        font-size: 40px;
      }
      span {
        font-size: 30px;
      }
    }
  }
}
</style>
