<template>
    <div class="container">
        <div class="header-image"></div>
        <div class="title" data-aos="fade-up" data-aos-delay="100"><h2>Events</h2></div>
        <div class="events-container">
            <h3 data-aos="fade-in" data-aos-delay="200">Event Name {{ date }}<span><br/>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor <br/>incididunt ut labore et dolore magna aliqua. Hac habitasse platea dictumst quisque.</span></h3>
            <h3 data-aos="fade-in" data-aos-delay="100">Event Name {{ date }}<span><br/>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor <br/>incididunt ut labore et dolore magna aliqua. Hac habitasse platea dictumst quisque.</span></h3>
        </div>
    </div>
</template>
<script>
export default {
    name: "Events",
    props: {
      date: String,
    }   
}
</script>
<style scoped lang="scss">
.container {
    position: relative;
    height: 160vh;
            background-image: linear-gradient(#2C2C50, #2C2C50);
    color: rgb(247, 247, 247);
    z-index: 1;
    h2 {
        padding-top: 300px;
        font-size: 80px;
    }
}
.header-image {
  background-image: url("~@/assets/wave-down.svg");
  background-repeat: no-repeat;
  background-size: contain;
  background-position: top;
  height: 100vh;
  width: 100%;
  top: -15%;
  z-index: -1;
  transform: scaleX(-1);
  position: absolute;

}
.events-container {
    height: 90vh;
    h3 {
    justify-content: center;
    padding-top: 100px;
    padding-bottom: 200px;
    line-height: 50px;
    font-size: 40px;
    span {
    font-size: 20px;
    }
    }
}
@media only screen and (min-device-width: 400px) and (max-device-width: 480px) {
    .container {
        height: 180vh;
    }
    .events-container {
        h3 {
            padding-bottom: 50px;
        }
    }
}
@media only screen and (min-device-width: 200px) and (max-device-width: 400px) {
    .container {
        height: 240vh;
    }
    .events-container {
        h3 {
            padding-bottom: 50px;
        }
    }
    .header-image {
  top: 0%;

}
}
</style>