<template>
    <div>
        <div class="titleLeft" data-aos="fade-up" data-aos-delay="100"><h2>About SCP:ET</h2><p>Based off of the 2012 horror game SCP: Containment Breach. Partner up or compete against your friends to explore the vast facility as well as gather useful, unknown, and potentially dangerous items to assist your escape and evade the potentially dangerous anomalies that roam the locked down facility.</p></div>
        <div class="titleRight" data-aos="fade-up" data-aos-delay="100"><h2>The plot</h2><p>Before the events of the game take place, several of the Foundation's sites and sectors were attacked, which caused several Euclid and Keter SCPs to be temporarily relocated to an unspecified site until repairs on the previous facilities are completed. It was unable to handle the quantity of SCPs it currently possessed.</p></div>
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
div {
    position: relative;
    display: flex;
    height: 70vh;
    top: 20%;
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
div {
    height: 120vh;
    .titleLeft {
        h2 {
            font-size: 30px;
        }
        p {
                font-size: 13px;
        }
    }
        .titleRight {
        h2 {
            font-size: 30px;
        }
        p {
                font-size: 13px;
        }
    }
}
}
</style>