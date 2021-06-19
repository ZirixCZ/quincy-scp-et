<template>
    <div class="container">
        <div class="title"><h2>Events</h2></div>
        <div class="events-container">
            <h3>Event Name {{ date }}<span><br/>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. <br/>Hac habitasse platea dictumst quisque.</span></h3>
            <h3>Event Name {{ date }}<span><br/>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. <br/>Hac habitasse platea dictumst quisque.</span></h3>
        </div>
    </div>
</template>
<script>
export default {
    name: "Events",
    props: {
      date: String,
    }   
}
</script>
<style scoped lang="scss">
.container {
    position: relative;
    height: 130vh;
    h2 {
        font-size: 80px;
    }
}
.events-container {
    height: 80vh;
    h3 {
    justify-content: center;
    padding-top: 100px;
    padding-bottom: 200px;
    line-height: 50px;
    font-size: 40px;
    span {
    font-size: 20px;
    }
    }
}
@media only screen and (min-device-width: 320px) and (max-device-width: 480px) {
    .container {
        height: 170vh;
    }
    .events-container {
        h3 {
            padding-bottom: 50px;
        }
    }
}
</style>