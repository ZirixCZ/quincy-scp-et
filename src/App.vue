<template>
  <router-view />
</template>


<script>
/*import axios from 'axios'
export default {
  name: 'App',
  data() {
    return {
    }
  },
  mounted: function () {
   axios.get('http://localhost:8080/api/ServerInfo/HostApi/Servers?key=K+I+Z1MNnHE=')
  .then(response => console.log(response.data))
  .catch(error => console.error(error));
  }}*/
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Noto+Sans:ital,wght@0,400;0,700;1,400;1,700&family=Open+Sans:ital,wght@0,300;0,400;0,600;0,700;0,800;1,300;1,400;1,600;1,700;1,800&family=Roboto:ital,wght@0,100;0,300;0,400;0,500;0,700;0,900;1,100;1,300;1,400;1,500;1,700;1,900&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Benne&family=Open+Sans:wght@300&family=Oswald:wght@200&family=Roboto:wght@100&display=swap');
$fontColor: #2c3e50;
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: $fontColor;
}
#app, html {
  background-color:rgb(250, 250, 250);
}
body,html {
  height: 100%;
  width: 100%;
  margin: 0;
  box-sizing: border-box;
}

/*scrollbar*/
::-webkit-scrollbar {
    -webkit-appearance: none;
}
::-webkit-scrollbar:vertical {
    width: 7px;
}
::-webkit-scrollbar:horizontal {
    height: 10px;
}
::-webkit-scrollbar-thumb {
    background-color: #0e141a;
}
::-webkit-scrollbar-track {
    background-color: #ffffff;
}
/*selection*/
::-moz-selection { /* Code for Firefox */
    color: rgb(255, 255, 255);
    background: rgb(20, 24, 32);
}  
::selection {
    color: rgb(255, 255, 255);
    background: rgb(20, 24, 32);
}
</style>
