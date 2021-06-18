<template>
        <div class="faq-container">
            <div class="faq-title"><h2>Frequently Asked Questions <i class="fas fa-question-circle"></i></h2></div>
            <ul><li>Is the game free?<span><br/>- Yes, the game is free. <a href="https://store.steampowered.com/app/1394270/SCP_Escape_Together/">SCP:ET</a></span></li>
            <li>How can I play the game with my friends?<span><br/>- Click on the serverlist in the main menu and connect to a server.</span></li>
            <li>Is the game a cryptocurrency miner?<span><br/>- No, it is not a miner.</span></li>
            <li>Is there an official discord server for the game?<span><br/>- Yes, there is. <a href="https://discord.gg/Y6ZSPwWSe6">SCP:ET Discord server</a></span></li>
            <li>Which SCPs/Items from the original game can I currently find in SCP:ET?<span><br/>- You can find the list of all SCPs and Items currently in the game <router-link to="SCP">here.</router-link></span></li></ul>
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
    height: 100vh;
    li {
    flex-direction: column;
    position: relative;
    display: flex;
    text-align: left;
    align-items: baseline;
    justify-content: center;
    list-style-type: none;
    padding-left: 300px;
    width: 100%;
    font-size: 25px;
    font-weight: 400;
    top: 30%;
    span {
    list-style-type: none;
    padding-bottom: 150px;
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
    font-size: 80px;
    font-weight: 300;
    top: 0;
    margin: 0;
}
  @media only screen and (min-device-width: 320px) and (max-device-width: 480px) {
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
</style>