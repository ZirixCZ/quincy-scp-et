<template>
  <div class="scp-picture-title">
    <h2><span>SCPs</span></h2>
    <h4>
      SCPs are objects/beings/places that break natural law like anti-gravity.
      SCPs can be classified to either Safe, Euclid and Keter.<br /><b>Safe</b>
      = Known and is easily controlled <br /><b>Euclid</b> = Not known well and
      need more attention than Safe SCPs <br /><b>Keter</b> = Known and unknown
      objects/beings that are to dangerous and must be watched and monitored
      24/7
    </h4>
  </div>
  <div class="scp-picture-container">
    <div class="doctor"><a>SCP-049</a></div>
    <div class="peanut"><a>SCP-173</a></div>
    <div class="dog"><a>SCP-939</a></div>
    <div class="larry"><a>SCP-106</a></div>
    <div class="zombie"><a>SCP-049-2</a></div>
    <div class="infection"><a>SCP-008</a></div>
    <div class="themachine"><a>SCP-914</a></div>
  </div>
  <div class="item-picture-title">
    <h2 data-aos="fade-up" data-aos-delay="50"><span>Items</span></h2>
    <h4 data-aos="fade-up" data-aos-delay="150">
      Those items had been left over after the original facility personal
      evacuated. Use those items wisely, your life is dependent on them. You can
      find them being scattered over the facility.
    </h4>
  </div>
  <div class="item-picture-container">
    <div class="lvl1"><a>Level 1 Keycard</a></div>
    <div class="lvl2"><a>Level 2 Keycard</a></div>
    <div class="lvl3"><a>Level 3 Keycard</a></div>
    <div class="lvl4"><a>Level 4 Keycard</a></div>
    <div class="lvl5"><a>Level 5 Keycard</a></div>
    <div class="snav"><a>S-Nav</a></div>
    <div class="medkit"><a>First Aid Kit</a></div>
  </div>
  <div class="scpitem-picture-title">
    <h2 data-aos="fade-up" data-aos-delay="50"><span>scpitems</span></h2>
    <h4 data-aos="fade-up" data-aos-delay="150">
      Those SCPs do not do anything on their own, they are classed as "safe." Do
      not get fooled by the peaceful class name.
    </h4>
  </div>
  <div class="scpitem-picture-container">
    <div class="thekey"><a>SCP-860</a></div>
    <div class="themask"><a>SCP-1499</a></div>
    <div class="thering"><a>SCP-714</a></div>
    <div class="encyclopedia"><a>SCP-1025</a></div>
  </div>
</template>
<script>
//Note: added new objects, do not forget to link their scp-wiki pages.
export default {
  name: "PictureSCP",
};
</script>
<style scoped lang="scss">
.scp-picture-title {
  font-family: "Roboto", sans-serif;
  position: relative;
  display: flex;
  text-align: center;
  align-items: center;
  justify-content: center;
  font-size: 30px;
  top: 0%;
  /*border-bottom: 1px solid white;*/
  h2 {
    color: white;
    font-size: 80px;
    font-weight: 300;
    padding-bottom: 200px;
    span {
      border-bottom: 4px solid rgb(238, 238, 238);
      padding-bottom: 7px;
      border-radius: 6px;
    }
  }
  h4 {
    width: 50%;
    top: 40%;
    color: white;
    position: absolute;
    line-height: 75px;
    font-size: 20px;
    font-weight: 200;
    letter-spacing: 0.75px;
  }
}
.item-picture-title {
  font-family: "Roboto", sans-serif;
  position: relative;
  display: flex;
  text-align: center;
  align-items: center;
  justify-content: center;
  font-size: 30px;
  top: 3%;
  /*border-bottom: 1px solid white;*/
  h2 {
    color: white;
    font-size: 80px;
    font-weight: 300;
    padding-bottom: 200px;
    span {
      border-bottom: 4px solid rgb(238, 238, 238);
      padding-bottom: 7px;
      border-radius: 6px;
    }
  }
  h4 {
    width: 50%;
    top: 40%;
    color: white;
    position: absolute;
    line-height: 75px;
    font-size: 20px;
    font-weight: 200;
    letter-spacing: 0.75px;
  }
}
.scpitem-picture-title {
  font-family: "Roboto", sans-serif;
  position: relative;
  display: flex;
  text-align: center;
  align-items: center;
  justify-content: center;
  font-size: 30px;
  top: 3%;
  /*border-bottom: 1px solid white;*/
  h2 {
    color: white;
    font-size: 80px;
    font-weight: 300;
    padding-bottom: 200px;
    span {
      border-bottom: 4px solid rgb(238, 238, 238);
      padding-bottom: 7px;
      border-radius: 6px;
    }
  }
  h4 {
    width: 50%;
    top: 40%;
    color: white;
    position: absolute;
    line-height: 75px;
    font-size: 20px;
    font-weight: 200;
    letter-spacing: 0.75px;
  }
}
.scp-picture-container {
  position: relative;
  display: grid;
  text-align: center;
  grid-template-columns: 400px 400px 400px;
  grid-template-rows: 400px 400px 400px;
  grid-gap: 10px 100px;
  font-size: 40px;
  padding-left: 330px;
  font-weight: 200;
  height: 150vh;
  top: 5%;
}
.doctor {
  background-image: url("~@/assets/scpet/scpimages/scpetdoctor.png");
  background-repeat: no-repeat;
  background-size: cover;
  transition: 0.3s ease-in-out;
  cursor: pointer;
  filter: grayscale(1) brightness(100%);
  width: 200px;
  height: 200px;
  border-radius: 5px;
}
.doctor:hover {
  filter: grayscale(0);
}
.doctor a {
  font-family: "Open Sans", sans-serif;
  position: relative;
  top: 105%;
  font-size: 20px;
  font-weight: 400;
  color: rgb(255, 255, 255);
  text-decoration: none;
}
.peanut {
  background-image: url("~@/assets/scpet/scpimages/scpetpeanut.png");
  background-repeat: no-repeat;
  background-size: cover;
  transition: 0.3s ease-in-out;
  cursor: pointer;
  filter: grayscale(1) brightness(100%);
  width: 200px;
  height: 200px;
  border-radius: 5px;
}
.peanut:hover {
  filter: grayscale(0);
}
.peanut a {
  font-family: "Open Sans", sans-serif;
  position: relative;
  top: 105%;
  font-size: 20px;
  font-weight: 400;
  color: rgb(255, 255, 255);
  text-decoration: none;
}
.dog {
  background-image: url("~@/assets/scpet/scpimages/scpetdog.png");
  background-repeat: no-repeat;
  background-size: cover;
  transition: 0.3s ease-in-out;
  cursor: pointer;
  filter: grayscale(1) brightness(100%);
  width: 200px;
  height: 200px;
  border-radius: 5px;
}
.dog:hover {
  filter: grayscale(0);
}
.dog a {
  font-family: "Open Sans", sans-serif;
  position: relative;
  top: 105%;
  font-size: 20px;
  font-weight: 400;
  color: rgb(255, 255, 255);
  text-decoration: none;
}
.larry {
  background-image: url("~@/assets/scpet/scpimages/scpetlarry.png");
  background-repeat: no-repeat;
  background-size: cover;
  transition: 0.3s ease-in-out;
  cursor: pointer;
  filter: grayscale(1) brightness(100%);
  width: 200px;
  height: 200px;
  border-radius: 5px;
}
.larry:hover {
  filter: grayscale(0);
}
.larry a {
  font-family: "Open Sans", sans-serif;
  position: relative;
  top: 105%;
  font-size: 20px;
  font-weight: 400;
  color: rgb(255, 255, 255);
  text-decoration: none;
}
.infection {
  background-image: url("~@/assets/scpet/scpimages/scpetinfection.png");
  background-repeat: no-repeat;
  background-size: cover;
  transition: 0.3s ease-in-out;
  cursor: pointer;
  filter: grayscale(1) brightness(100%);
  width: 200px;
  height: 200px;
  border-radius: 5px;
}
.infection:hover {
  filter: grayscale(0);
}
.infection a {
  font-family: "Open Sans", sans-serif;
  position: relative;
  top: 105%;
  font-size: 20px;
  font-weight: 400;
  color: rgb(255, 255, 255);
  text-decoration: none;
}
.zombie {
  background-image: url("~@/assets/scpet/scpimages/scpetzombie.png");
  background-repeat: no-repeat;
  background-size: cover;
  transition: 0.3s ease-in-out;
  cursor: pointer;
  filter: grayscale(1) brightness(100%);
  width: 200px;
  height: 200px;
  border-radius: 5px;
}
.zombie:hover {
  filter: grayscale(0);
}
.zombie a {
  font-family: "Open Sans", sans-serif;
  position: relative;
  top: 105%;
  font-size: 20px;
  font-weight: 400;
  color: rgb(255, 255, 255);
  text-decoration: none;
}
.themachine {
  background-image: url("~@/assets/scpet/scpimages/914.png");
  background-repeat: no-repeat;
  background-size: contain;
  transition: 0.3s ease-in-out;
  cursor: pointer;
  filter: grayscale(1) brightness(100%);
  width: 200px;
  height: 200px;
  border-radius: 5px;
}
.themachine:hover {
  filter: grayscale(0);
}
.themachine a {
  font-family: "Open Sans", sans-serif;
  position: relative;
  top: 105%;
  font-size: 20px;
  font-weight: 400;
  color: rgb(255, 255, 255);
  text-decoration: none;
}
.item-picture-container {
  position: relative;
  display: grid;
  text-align: center;
  grid-template-columns: 400px 400px 400px;
  grid-template-rows: 400px 400px 400px;
  grid-gap: 10px 100px;
  font-size: 40px;
  padding-left: 330px;
  font-weight: 200;
  height: 200vh;
  top: 9%;
}
.lvl1 {
  background-image: url("~@/assets/scpet/itemimages/level1keycard.png");
  background-repeat: no-repeat;
  background-size: contain;
  transition: 0.3s ease-in-out;
  cursor: pointer;
  filter: grayscale(1) brightness(100%);
  width: 200px;
  height: 200px;
  border-radius: 5px;
}
.lvl1:hover {
  filter: grayscale(0) brightness(100%);
}
.lvl1 a {
  font-family: "Open Sans", sans-serif;
  position: relative;
  top: 105%;
  font-size: 20px;
  font-weight: 400;
  color: rgb(255, 255, 255);
  text-decoration: none;
}
.lvl2 {
  background-image: url("~@/assets/scpet/itemimages/level2keycard.png");
  background-repeat: no-repeat;
  background-size: contain;
  transition: 0.3s ease-in-out;
  cursor: pointer;
  filter: grayscale(1) brightness(100%);
  width: 200px;
  height: 200px;
  border-radius: 5px;
}
.lvl2:hover {
  filter: grayscale(0) brightness(90%);
}
.lvl2 a {
  font-family: "Open Sans", sans-serif;
  position: relative;
  top: 105%;
  font-size: 20px;
  font-weight: 400;
  color: rgb(255, 255, 255);
  text-decoration: none;
}
.lvl3 {
  background-image: url("~@/assets/scpet/itemimages/level3keycard.png");
  background-repeat: no-repeat;
  background-size: contain;
  transition: 0.3s ease-in-out;
  cursor: pointer;
  filter: grayscale(1) brightness(100%);
  width: 200px;
  height: 200px;
  border-radius: 5px;
}
.lvl3:hover {
  filter: grayscale(0) brightness(90%);
}
.lvl3 a {
  font-family: "Open Sans", sans-serif;
  position: relative;
  top: 105%;
  font-size: 20px;
  font-weight: 400;
  color: rgb(255, 255, 255);
  text-decoration: none;
}
.lvl4 {
  background-image: url("~@/assets/scpet/itemimages/level4keycard.png");
  background-repeat: no-repeat;
  background-size: contain;
  transition: 0.3s ease-in-out;
  cursor: pointer;
  filter: grayscale(1) brightness(90%);
  width: 200px;
  height: 200px;
  border-radius: 5px;
}
.lvl4:hover {
  filter: grayscale(0) brightness(90%);
}
.lvl4 a {
  font-family: "Open Sans", sans-serif;
  position: relative;
  top: 105%;
  font-size: 20px;
  font-weight: 400;
  color: rgb(255, 255, 255);
  text-decoration: none;
}
.lvl5 {
  background-image: url("~@/assets/scpet/itemimages/level5keycard.png");
  background-repeat: no-repeat;
  background-size: contain;
  transition: 0.3s ease-in-out;
  cursor: pointer;
  filter: grayscale(1) brightness(100%);
  width: 200px;
  height: 200px;
  border-radius: 5px;
}
.lvl5:hover {
  filter: grayscale(0) brightness(90%);
}
.lvl5 a {
  font-family: "Open Sans", sans-serif;
  position: relative;
  top: 105%;
  font-size: 20px;
  font-weight: 400;
  color: rgb(255, 255, 255);
  text-decoration: none;
}
.snav {
  background-image: url("~@/assets/scpet/itemimages/snav.png");
  background-repeat: no-repeat;
  background-size: contain;
  transition: 0.3s ease-in-out;
  cursor: pointer;
  filter: grayscale(1) brightness(100%);
  width: 200px;
  height: 200px;
  border-radius: 5px;
}
.snav:hover {
  filter: grayscale(0) brightness(90%);
}
.snav a {
  font-family: "Open Sans", sans-serif;
  position: relative;
  top: 105%;
  font-size: 20px;
  font-weight: 400;
  color: rgb(255, 255, 255);
  text-decoration: none;
}
.medkit {
  background-image: url("~@/assets/scpet/itemimages/firstaidkit.png");
  background-repeat: no-repeat;
  background-size: contain;
  transition: 0.3s ease-in-out;
  cursor: pointer;
  filter: grayscale(1) brightness(100%);
  width: 200px;
  height: 200px;
  border-radius: 5px;
}
.medkit:hover {
  filter: grayscale(0) brightness(90%);
}
.medkit a {
  font-family: "Open Sans", sans-serif;
  position: relative;
  top: 105%;
  font-size: 20px;
  font-weight: 400;
  color: rgb(255, 255, 255);
  text-decoration: none;
}
.scpitem-picture-container {
  position: relative;
  display: grid;
  text-align: center;
  grid-template-columns: 400px 400px 400px;
  grid-template-rows: 400px 400px 400px;
  grid-gap: 10px 100px;
  font-size: 40px;
  padding-left: 330px;
  font-weight: 200;
  height: 100vh;
  top: 9%;
}
.encyclopedia {
  background-image: url("~@/assets/scpet/itemscp/encyclopedia.png");
  background-repeat: no-repeat;
  background-size: contain;
  transition: 0.3s ease-in-out;
  cursor: pointer;
  filter: grayscale(1) brightness(100%);
  width: 200px;
  height: 200px;
  border-radius: 5px;
}
.encyclopedia:hover {
  filter: grayscale(0) brightness(100%);
}
.encyclopedia a {
  font-family: "Open Sans", sans-serif;
  position: relative;
  top: 105%;
  font-size: 20px;
  font-weight: 400;
  color: rgb(255, 255, 255);
  text-decoration: none;
}
.thekey {
  background-image: url("~@/assets/scpet/itemscp/thekey.png");
  background-repeat: no-repeat;
  background-size: contain;
  transition: 0.3s ease-in-out;
  cursor: pointer;
  filter: grayscale(1) brightness(100%);
  width: 200px;
  height: 200px;
  border-radius: 5px;
}
.thekey:hover {
  filter: grayscale(0) brightness(90%);
}
.thekey a {
  font-family: "Open Sans", sans-serif;
  position: relative;
  top: 105%;
  font-size: 20px;
  font-weight: 400;
  color: rgb(255, 255, 255);
  text-decoration: none;
}
.themask {
  background-image: url("~@/assets/scpet/itemscp/themask.png");
  background-repeat: no-repeat;
  background-size: contain;
  transition: 0.3s ease-in-out;
  cursor: pointer;
  filter: grayscale(1) brightness(100%);
  width: 200px;
  height: 200px;
  border-radius: 5px;
}
.themask:hover {
  filter: grayscale(0) brightness(90%);
}
.themask a {
  font-family: "Open Sans", sans-serif;
  position: relative;
  top: 105%;
  font-size: 20px;
  font-weight: 400;
  color: rgb(255, 255, 255);
  text-decoration: none;
}
.thering {
  background-image: url("~@/assets/scpet/itemscp/thering.png");
  background-repeat: no-repeat;
  background-size: contain;
  transition: 0.3s ease-in-out;
  cursor: pointer;
  filter: grayscale(1) brightness(90%);
  width: 200px;
  height: 200px;
  border-radius: 5px;
}
.thering:hover {
  filter: grayscale(0) brightness(90%);
}
.thering a {
  font-family: "Open Sans", sans-serif;
  position: relative;
  top: 105%;
  font-size: 20px;
  font-weight: 400;
  color: rgb(255, 255, 255);
  text-decoration: none;
}
@media only screen and (min-device-width: 320px) and (max-device-width: 480px) {
  .scp-picture-container {
    grid-template-columns: 400px;
    grid-template-rows: 400px 400px 400px 400px 400px 400px;
    height: 700vh;
    top: 7%;
    padding-left: 75px;
  }
  .item-picture-title {
    top: 0%;
  }
  .item-picture-container {
    grid-template-columns: 400px;
    grid-template-rows: 400px 400px 400px 400px 400px 400px;
    height: 290vh;
    padding-left: 75px;
  }
  .scpitem-picture-title {
    top: 20%;
  }
  .scpitem-picture-container {
    grid-template-columns: 400px;
    grid-template-rows: 400px 400px 400px 400px 400px 400px;
    height: 250vh;
    padding-left: 75px;
    top: 30%;
  }
}
@media screen and (min-device-width: 1200px) and (max-device-width: 1600px) and (-webkit-min-device-pixel-ratio: 1) {
  .scp-picture-container {
    grid-template-columns: 400px 400px;
    grid-template-rows: 400px 400px 400px;
    height: 250vh;
  }
  .item-picture-container {
    grid-template-columns: 400px 400px;
    grid-template-rows: 400px 400px 400px 400px;
    height: 290vh;
  }
  .scpitem-picture-container {
    grid-template-columns: 400px 400px;
    grid-template-rows: 400px 400px 400px 400px;
    height: 250vh;
  }
}
/*scrollbar*/
::-webkit-scrollbar {
  -webkit-appearance: none;
}
::-webkit-scrollbar:vertical {
  width: 15px;
}
::-webkit-scrollbar:horizontal {
  height: 15px;
}
::-webkit-scrollbar-thumb {
  background-color: #1f2c38;
  border-radius: 5px;
}
::-webkit-scrollbar-track {
  border-radius: 10px;
  background-color: #f0f0f0;
}
</style>
