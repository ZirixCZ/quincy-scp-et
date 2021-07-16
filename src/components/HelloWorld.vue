<template>
    <div class="title-div">
      <div class="header-image" data-aos="fade-in" data-aos-delay="200"></div>
      <h1 data-aos="fade-up" data-aos-delay="50">Quincy's Party</h1>
      <div class="button-wrapper" data-aos="fade-up" data-aos-delay="250" onclick="location.href='https://discord.com/invite/F2zFuaB';"><button>join us!</button></div>
      <h2 data-aos="fade-up" data-aos-delay="150">There are <span>{{ players }}</span> people playing right now.</h2>
    </div>
  <div class="nav">
    <div class="nav-item" data-aos="fade-right" data-aos-delay="700"><button class="switch nav-item" @click="darkThemeSwitch"><i class="fas fa-moon"></i></button></div>
    <div class="nav-item" data-aos="fade-right" data-aos-delay="500" onclick="location.href='https://www.reddit.com/r/QuincysSCPparty/';"><button class="nav-item"><i class="fab fa-reddit-alien"></i></button></div>
    <div class="nav-item" data-aos="fade-right" data-aos-delay="300" onclick="location.href='https://discord.com/invite/F2zFuaB';"><button class="nav-item"><i class="fab fa-discord"></i></button></div>
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
      lastScrollPosition: 0,
    }
  },
  async mounted () {
    const response = await axios.get('https://www.quincyet.ga/api/ServerInfo/HostApi/Servers?key=' + process.env.VUE_APP_ROOT_API)
    this.players = response.data.Servers[0].PlayerCount
  },
      methods: {
  //https://dev.to/nuculabs_dev/simple-dark-theme-switch-with-vue-js-59hp - I got the code there
    
    // links the dark theme
    _addDarkTheme() {
      let darkThemeLinkEl = document.createElement("link");
      darkThemeLinkEl.setAttribute("rel", "stylesheet");
      darkThemeLinkEl.setAttribute("href", "/styles/darktheme.css");
      darkThemeLinkEl.setAttribute("id", "dark-theme-style");

      let docHead = document.querySelector("head");
      docHead.append(darkThemeLinkEl);
    },
    // unlinks the dark theme
    _removeDarkTheme() {
      let darkThemeLinkEl = document.querySelector("#dark-theme-style");
      let parentNode = darkThemeLinkEl.parentNode;
      parentNode.removeChild(darkThemeLinkEl);
    },
    // switches between linked and unlinked
    darkThemeSwitch() {
      let darkThemeLinkEl = document.querySelector("#dark-theme-style");
      if (!darkThemeLinkEl) {
        this._addDarkTheme()
      } else {
        this._removeDarkTheme()
      }
    }
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
    font-family: 'Montserrat', sans-serif;
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
    font-family: 'Montserrat', sans-serif;
    position: relative;
    width: 250px;
    height: 50px;
    font-weight: 600;
    word-spacing: 3px;
    letter-spacing: 1px;
    font-size: 15px;
    text-transform: uppercase;
    background-color:rgb(250, 250, 250);
    border: none;
    outline: none;
    color:#222222;
    cursor: pointer;
    border-radius: 5px;
    transition: 0.2s ease-in-out;
    box-shadow: #1e2a36 0px 0px 20px;
    &:hover {
      width: 220px;
      letter-spacing: 2px;

    }
  }
  }
}
  .nav {
    position: absolute;
    display: flex;
    top: 0%;
    width: 100%;
    height: 10vh;
    align-items: center;
    justify-content: flex-start;
    .nav-item {
      padding-left: 5%;
    }
    .nav-item {
      background: none;
      border: none;
      text-decoration: none;
      color: white;
      font-size: 30px;
      padding-left: 5%;
      transition: 0.3s;
      cursor: pointer;
      &:hover {
        transform: scale(1.1);
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
    @media screen 
  and (min-device-width: 2400px) 
  and (max-device-width: 4000px) 
  and (-webkit-min-device-pixel-ratio: 1) {
        .title-div {
      h1 {
        font-size: 240px;
      }
      h2 {
        top: 38%;
        font-size: 35px;
      }


        .button-wrapper {
  button {
    width: 300px;
    height: 60px;
    font-size: 18px;
    &:hover {
      width: 270px;

    }
  }
  }
    }
      .nav {
    .nav-item {
      font-size: 40px;
      cursor: pointer;
  }
  }
  }
</style>
