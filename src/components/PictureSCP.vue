<template>
            <div class="scp-picture-title"><h2><span>SCPs</span></h2><h4>SCPs are anomalies that have been captured by the Foundation.

SCPs are stored within numerous sites owned by the Foundation across the world; these sites including places such as Site-48, Site-17 and Site-02, the last site being where SCP SL takes place.

While some anomalies can either be harmful or hostile, others can be very beneficial if used correctly. The following SCPs are found in-game.</h4></div>
        <div class="scp-picture-container">
            <div class="doctor" onclick="location.href='http://www.scpwiki.com/scp-049';"><a href="http://www.scpwiki.com/scp-049" target="_blank">SCP-049</a></div>
            <div class="peanut" onclick="location.href='http://www.scpwiki.com/scp-173';"><a href="http://www.scpwiki.com/scp-173" target="_blank">SCP-173</a></div>
            <div class="dog" onclick="location.href='http://www.scpwiki.com/scp-939';"><a href="http://www.scpwiki.com/scp-939" target="_blank">SCP-939</a></div>
            <div class="larry" onclick="location.href='http://www.scpwiki.com/scp-106';"><a href="http://www.scpwiki.com/scp-106" target="_blank">SCP-106</a></div>
            <div class="zombie" onclick="location.href='http://www.scpwiki.com/scp-049';"><a href="http://www.scpwiki.com/scp-049" target="_blank">SCP-049-2</a></div>
            <div class="infection" onclick="location.href='http://www.scpwiki.com/scp-008';"><a href="http://www.scpwiki.com/scp-008" target="_blank">SCP-008</a></div>
       </div>
                   <div class="item-picture-title"><h2><span>Items</span></h2><h4>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</h4></div>
       <div class="item-picture-container">
            <div class="itemname1" onclick="location.href='http://www.scpwiki.com/scp-049';"><a href="http://www.scpwiki.com/scp-049" target="_blank">Itemname1</a></div>
            <div class="itemname2" onclick="location.href='http://www.scpwiki.com/scp-173';"><a href="http://www.scpwiki.com/scp-173" target="_blank">Itemname2</a></div>
            <div class="itemname3" onclick="location.href='http://www.scpwiki.com/scp-939';"><a href="http://www.scpwiki.com/scp-939" target="_blank">Itemname3</a></div>
            <div class="itemname4" onclick="location.href='http://www.scpwiki.com/scp-106';"><a href="http://www.scpwiki.com/scp-106" target="_blank">Itemname4</a></div>
            <div class="itemname5" onclick="location.href='http://www.scpwiki.com/scp-049';"><a href="http://www.scpwiki.com/scp-049" target="_blank">Itemname5</a></div>
            <div class="itemname6" onclick="location.href='http://www.scpwiki.com/scp-008';"><a href="http://www.scpwiki.com/scp-008" target="_blank">Itemname6</a></div>
       </div>            
</template>
<script>
export default {
  name: "PictureSCP",
};
</script>
<style scoped lang="scss">
.scp-picture-title {
    font-family: 'Roboto', sans-serif;
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
    border-bottom:4px solid rgb(238, 238, 238);
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
    font-family: 'Roboto', sans-serif;
    position: relative;
    display: flex;
    text-align: center;
    align-items: center;
    justify-content: center;
    font-size: 30px;
    top: 10%;
    /*border-bottom: 1px solid white;*/
    h2 {
    color: white;
    font-size: 80px;
    font-weight: 300;
    padding-bottom: 200px;
    span {
    border-bottom:4px solid rgb(238, 238, 238);
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
    height: 100vh;
    top: 12%;
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
    filter: grayscale(1) brightness(90%);
}
.doctor a {
    font-family: 'Open Sans', sans-serif;;
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
    filter: grayscale(1) brightness(90%);
}
.peanut a {
    font-family: 'Open Sans', sans-serif;;
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
    filter: grayscale(1) brightness(90%);
}
.dog a {
    font-family: 'Open Sans', sans-serif;;
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
    filter: grayscale(1) brightness(90%);
}
.larry a {
    font-family: 'Open Sans', sans-serif;;
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
    filter: grayscale(1) brightness(90%);
}
.infection a {
    font-family: 'Open Sans', sans-serif;;
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
    filter: grayscale(1) brightness(90%);
}
.zombie a {
    font-family: 'Open Sans', sans-serif;;
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
    height: 100vh;
    top: 23%;
}
.itemname1 {
    background-image: url("~@/assets/scpet/itemimages/level1keycard.png");
    background-repeat: no-repeat;
    background-size: cover;
    transition: 0.3s ease-in-out;
    cursor: pointer;
    filter: grayscale(1) brightness(100%);
    width: 200px;
    height: 200px;
    border-radius: 5px;
}
.itemname1:hover {
    filter: grayscale(1) brightness(90%);
}
.itemname1 a {
    font-family: 'Open Sans', sans-serif;;
    position: relative;
    top: 105%;
    font-size: 20px;
    font-weight: 400;
    color: rgb(255, 255, 255);
    text-decoration: none;
}
.itemname2 {
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
.itemname2:hover {
    filter: grayscale(1) brightness(90%);
}
.itemname2 a {
    font-family: 'Open Sans', sans-serif;;
    position: relative;
    top: 105%;
    font-size: 20px;
    font-weight: 400;
    color: rgb(255, 255, 255);
    text-decoration: none;
}
.itemname3 {
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
.itemname3:hover {
    filter: grayscale(1) brightness(90%);
}
.itemname3 a {
    font-family: 'Open Sans', sans-serif;;
    position: relative;
    top: 105%;
    font-size: 20px;
    font-weight: 400;
    color: rgb(255, 255, 255);
    text-decoration: none;
}
.itemname4 {
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
.itemname4:hover {
    filter: grayscale(1) brightness(90%);
}
.itemname4 a {
    font-family: 'Open Sans', sans-serif;;
    position: relative;
    top: 105%;
    font-size: 20px;
    font-weight: 400;
    color: rgb(255, 255, 255);
    text-decoration: none;
}
.itemname5 {
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
.itemname5:hover {
    filter: grayscale(1) brightness(90%);
}
.itemname5 a {
    font-family: 'Open Sans', sans-serif;;
    position: relative;
    top: 105%;
    font-size: 20px;
    font-weight: 400;
    color: rgb(255, 255, 255);
    text-decoration: none;
}
.itemname6 {
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
.itemname6:hover {
    filter: grayscale(1) brightness(90%);
}
.itemname6 a {
    font-family: 'Open Sans', sans-serif;;
    position: relative;
    top: 105%;
    font-size: 20px;
    font-weight: 400;
    color: rgb(255, 255, 255);
    text-decoration: none;
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