<template>
<transition appear>
<div class="title-div">
    <h1>{{ title }}</h1>
    <button>join us</button>
    <h2>There is <span>xx</span> active people right now.</h2>
  </div>
</transition>
</template>

<script>
export default {
  name: "HelloWorld",
    data () {
    return {
      showPara: true,
      lastScrollPosition: 0
    }
  },
  props: {
    title: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.title-div {
  position: relative;
  text-align: center;
  height: 100vh;
  h1 {
    position: relative;
    top: 30%;
    font-size: 120px;
  }
  h2 {
    position: relative;
    top: 25%;
    span {
      color: rgb(212, 71, 71);
    }
  }
  button {
    position: relative;
    top: 40%;
    width: 250px;
    height: 50px;
    word-spacing: 10px;
        letter-spacing: 2px;
    background-color: white;
    border-color: #2c3e50;
    cursor: pointer;
    transition: 0.2s ease-in-out;
    &:hover {
      width: 220px;
      letter-spacing: 3px;

    }
  }
}
@media only screen and (min-device-width: 320px) and (max-device-width: 480px) {
    .title-div {
      h1 {
        font-size: 40px;
      }
      h2 {
        top: 20%;
        font-size: 20px;
      }
    }
}
</style>
