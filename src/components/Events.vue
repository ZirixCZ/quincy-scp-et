<template>
    <div class="container">
        <div class="title" data-aos="fade-up" data-aos-delay="100"><h2>Events</h2></div>
        <div class="events-container">
            <h3 data-aos="fade-in" data-aos-delay="200">Event Name {{ date }}<span><br/>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor <br/>incididunt ut labore et dolore magna aliqua. Hac habitasse platea dictumst quisque.</span></h3>
            <h3 data-aos="fade-in" data-aos-delay="100">Event Name {{ date }}<span><br/>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor <br/>incididunt ut labore et dolore magna aliqua. Hac habitasse platea dictumst quisque.</span></h3>
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
@media only screen and (min-device-width: 400px) and (max-device-width: 480px) {
    .container {
        height: 180vh;
    }
    .events-container {
        h3 {
            padding-bottom: 50px;
        }
    }
}
@media only screen and (min-device-width: 200px) and (max-device-width: 400px) {
    .container {
        height: 240vh;
    }
    .events-container {
        h3 {
            padding-bottom: 50px;
        }
    }
}
</style>