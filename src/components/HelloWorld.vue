<template>
    <div class="title-div">
      <div class="header-image" data-aos="fade-in" data-aos-delay="200"></div>
      <h1 data-aos="fade-up" data-aos-delay="50">QuincyET Party</h1>
      <div class="button-wrapper" data-aos="fade-up" data-aos-delay="250"><button>join us</button></div>
      <h2 data-aos="fade-up" data-aos-delay="150">There is <span>{{ players }}</span> people playing right now.</h2>
    </div>
</template>

<script>
import axios from 'axios'
export default {
  name: "HelloWorld",
  data () {
    return {
      players: 0,
      showPara: true,
      lastScrollPosition: 0
    }
  },
  async mounted () {
    const response = await axios.get('http://localhost:8080/api/ServerInfo/HostApi/Servers?key=')
    this.players = response.data.Servers[0].PlayerCount
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.header-image {
  background-image: url("~@/assets/wawe-front.svg");
  background-repeat: no-repeat;
  background-size: contain;
  background-position: bottom;
  background-color: #2c3e50;
  height: 100vh;
  width: 100%;
  position: absolute;

}
.title-div {
  position: relative;
  text-align: center;
  height: 100vh;
  color: rgb(247, 247, 247);
  h1 {
    position: relative;
    top: 40%;
    font-size: 150px;
    filter: drop-shadow(1px 1px 50px rgba(0, 0, 0, 0.1));
    margin: 0;
  }
  h2 {
    position: relative;
    top: 40%;
    span {
      color: #4c8d6d;
      text-shadow: 2px 2px 10px rgba(0, 0, 0, 0.288);
    }
  }
  .button-wrapper {
    position: relative;
    top: 55%;
  button {
    position: relative;

    width: 250px;
    height: 50px;
    word-spacing: 10px;
    letter-spacing: 2px;
    background-color:rgb(250, 250, 250);
    border-color: #2c3e50;
    cursor: pointer;
    transition: 0.2s ease-in-out;
    &:hover {
      width: 220px;
      letter-spacing: 3px;

    }
  }
  }
}
@media only screen and (min-device-width: 320px) and (max-device-width: 480px) {
    .title-div {
      h1 {
        font-size: 40px;
      }
      h2 {
        top: 40%;
        font-size: 15px;
      }
    .button-wrapper {
        top: 60%;
  }
    }
}
  @media screen 
  and (min-device-width: 1200px) 
  and (max-device-width: 1600px) 
  and (-webkit-min-device-pixel-ratio: 1) {
    .title-div {
      h1 {
        font-size: 120px;
      }
      h2 {
        top: 38%;
        font-size: 20px;
      }
    }
  }
</style>
