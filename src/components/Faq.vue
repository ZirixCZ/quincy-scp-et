<template>
        <div class="faq-container">
            <div class="faq-title" data-aos="fade-up" data-aos-delay="100"><h2>Frequently Asked Questions <i class="fas fa-question-circle"></i></h2></div>
            <ul><li data-aos="fade-right" data-aos-delay="100">Is the game free?<span><br/>- Yes, the game is free. <a href="https://store.steampowered.com/app/1394270/SCP_Escape_Together/">SCP:ET</a></span></li>
            <li data-aos="fade-right" data-aos-delay="0">How can I play the game with my friends?<span><br/>- Click on the serverlist in the main menu and connect to a server.</span></li>
            <li data-aos="fade-right" data-aos-delay="0">Is the game a cryptocurrency miner?<span><br/>- No, it is not a miner.</span></li>
            <li data-aos="fade-right" data-aos-delay="0">Is there an official discord server for the game?<span><br/>- Yes, there is. <a href="https://discord.gg/Y6ZSPwWSe6">SCP:ET Discord server</a></span></li>
            <li data-aos="fade-right" data-aos-delay="0">Which SCPs/Items from the original game can I currently find in SCP:ET?<span><br/>- You can find the list of all SCPs and Items currently in the game <router-link to="List">here.</router-link></span></li></ul>
        </div>
</template>
<script>
export default {
  name: "Faq",
};
</script>
<style scoped lang="scss">
.faq-container {
    position: relative;
    display: flex;
    text-align: center;
    height: 150vh;
    color: rgb(247, 247, 247);
    background-image: linear-gradient(#2C2C50, #242442);
    margin: 0;
    li {
    flex-direction: column;
    position: relative;
    display: flex;
    text-align: left;
    align-items: baseline;
    justify-content: center;
    list-style-type: none;
    padding-left: 300px;
    width: 50%;
    font-size: 30px;
    font-weight: 400;
    top: 20%;
    a {
        color: rgb(89, 137, 201);
        text-decoration: none;
    }
    span {
    list-style-type: none;
    padding-bottom: 100px;
    font-size: 20px;
    font-weight: 300;
    }
    }
}
.faq-title {
    display: flex;
    text-align: center;
    position: absolute;
    justify-content: center;
    height: 100%;
    width: 100%;
}
.faq-title h2 {
    position: absolute;
    flex: 50%;
    font-size: 90px;
    padding-top: 100px;
    font-weight: 300;
    top: 0;
    margin: 0;
}
  @media only screen and (min-device-width: 320px) and (max-device-width: 480px) {
      .faq-container {
          height: 230vh;
          li {
              top: 10%;
              padding-left: 10px;
              width: 80%;
          }
      }
      .faq-title h2 {
          font-size: 40px;
      }
  }
  @media only screen and (min-device-width: 200px) and (max-device-width: 400px) {
      .faq-container {
          height: 290vh;
          li {
              top: 10%;
              padding-left: 10px;
              width: 80%;
          }
      }
      .faq-title h2 {
          font-size: 40px;
      }
}
  @media only screen and (min-device-width: 768px) and (max-device-width: 1024px) and (orientation: portrait) {
        .faq-container {
          height: 120vh;
          li {
              top: 40%;
              padding-left: 10px;
              width: 80%;
          }
      }
      .faq-title h2 {
          font-size: 40px;
      }
   
  }
    @media screen 
  and (min-device-width: 1200px) 
  and (max-device-width: 1600px) 
  and (-webkit-min-device-pixel-ratio: 1) {
      .faq-container {
          li {
              padding-left: 50px;
          }
      }
  }
</style>