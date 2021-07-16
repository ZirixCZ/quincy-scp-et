<template>
    <div class="container">
        <div class="titleLeft" data-aos="fade-up" data-aos-delay="100"><h2>About SCP:ET</h2><p>SCP: Escape Together is a multiplayer horror game created by a team of developers who all share the love for the SCP universe. The game is based off of the original 2012 SCP: Containment Breach, adds new features, support and possibilities.</p></div>
        <div class="titleRight" data-aos="fade-up" data-aos-delay="100"><h2>The plot</h2><p>The story takes places in an attacked facility. The attack caused several containment breaches on the Euclid and Keter levels. You are playing as a class-D personal, a test subject. You got left over and now have to find your way out.</p></div>
    </div>
</template>

<script>
export default {
  name: "InformationFlex",
  props: {
      titleLeft: String,
      titleRight: String,
      textLeft: String,
      textRight: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
body, html {
    width: 100%;
    height: 100%;
}
* {
    margin: 0;
    padding: 0;
}
.container {
    position: relative;
    display: flex;
    height: 25vh;
    top: 20%;
    z-index: 2;
    .titleLeft {
    display: flex;
    align-items: center;
    flex-direction: column;
    flex: 50%;
    width: 30px;
    h2 {
        font-size: 40px;
        padding-bottom: 30px;
    }
    p {
    text-align: justify;
    width: 60%; 
    font-size: 20px;
    letter-spacing: 1.5px;
    }
    }
    .titleRight {
    display: flex;
    align-items: center;
    flex-direction: column;
    flex: 50%;
    h2 {
    font-size: 40px;
    padding-bottom: 30px;
    }
    p {
    text-align: justify;
    width: 60%; 
    font-size: 20px;
    letter-spacing: 1.5px;
    }
    }
}
@media only screen and (min-device-width: 320px) and (max-device-width: 480px) {
.container {
    height: 100vh;
    flex-direction: column;
    p {
        font-weight: 600;
    }
    .titleLeft {
        width: 100%;
        h2 {
            font-size: 30px;
        }
        p {
                font-size: 15px;
                padding-bottom: 90px;
        }
    }
        .titleRight {
        width: 100%;
        h2 {
            font-size: 30px;
        }
        p {
                font-size: 15px;
        }
    }
}
}
@media only screen and (min-device-width: 320px) and (max-device-width: 360px) {
    .container {
    height: 130vh;
}
}
  @media screen 
  and (min-device-width: 2400px) 
  and (max-device-width: 4000px) 
  and (-webkit-min-device-pixel-ratio: 1) {
.container {
    .titleLeft {
    h2 {
        font-size: 60px;
    }
    p { 
    font-size: 25px;
    }
    }
    .titleRight {
    h2 {
    font-size: 60px;
    }
    p {
    font-size: 25px;
    }
    }
}}
</style>