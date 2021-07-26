<template>
  <div class="faq-container">
    <div class="faq-title" data-aos="fade-up" data-aos-delay="100">
      <h2>Frequently Asked Questions</h2>
    </div>
    <ul>
      <li data-aos="fade-right" data-aos-delay="100">
        Do I have to pay to play the game?<span
          ><br />- You do not, the game is free. You can download the game
          <a
            href="https://store.steampowered.com/app/1394270/SCP_Escape_Together/"
            >here.</a
          ></span
        >
      </li>
      <li data-aos="fade-right" data-aos-delay="0">
        Is it hard to play with my friends?<span
          ><br />- It is not hard at all! All you have to do, is go to the main
          menu, click on the server list and choose a server.</span
        >
      </li>
      <li data-aos="fade-right" data-aos-delay="0">
        I heard some people say the game is a cryptocurrency miner, is it
        true?<span
          ><br />- Absolutely not true. If you have a lower end machine,
          consider lowering the graphical settings. The game is still in Early
          Access and the developers are working on optimizing the game.</span
        >
      </li>
      <li data-aos="fade-right" data-aos-delay="0">
        Is there an official discord server for the game?<span
          ><br />- <a href="https://discord.gg/Y6ZSPwWSe6">This</a> is the
          official discord server for the game, enjoy it!</span
        >
      </li>
      <li data-aos="fade-right" data-aos-delay="0">
        Can I somewhere find the SCP objects currently foundable in the
        game?<span
          ><br />- I created
          <router-link to="List">this simple list</router-link> of all
          SCPs/Objets currently naturally foundable in the game. It will get
          replaced when the official SCP: Escape Together wiki is done.</span
        >
      </li>
    </ul>
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
  height: 200vh;
  color: rgb(247, 247, 247);
  background-image: linear-gradient(#2c2c50, #242442);
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
    padding-top: 75px;
    width: 50%;
    font-size: 30px;
    font-weight: 400;
    top: 20%;
    a {
      color: #add3ff;
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
  font-weight: 400;
  top: 0;
  margin: 0;
}
@media only screen and (min-device-width: 320px) and (max-device-width: 750px) {
  .faq-container {
    height: 350vh;
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
    height: 530vh;
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
    height: 270vh;
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
@media screen and (min-device-width: 1200px) and (max-device-width: 1600px) and (-webkit-min-device-pixel-ratio: 1) {
  .faq-container {
    height: 300vh;
    li {
      padding-left: 50px;
    }
  }
}
@media screen and (min-device-width: 2400px) and (max-device-width: 4000px) and (-webkit-min-device-pixel-ratio: 1) {
  .faq-container {
    height: 180vh;
    li {
      font-size: 40px;
      span {
        font-size: 30px;
      }
    }
  }
  .faq-title h2 {
    font-size: 120px;
  }
}
</style>
