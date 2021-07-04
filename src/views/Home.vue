<template>
  <div class="home">
    <HelloWorld />
    <InformationFlex />
    <Events date="4/12" event1="Event Name 1" event2="Event Name 2"/>
    <Faq />
    <Footer />
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";
import InformationFlex from "@/components/InformationFlex.vue";
import Faq from "@/components/Faq.vue";
import Events from "@/components/Events.vue";
import Footer from "@/components/Footer.vue";

export default {
  name: "Home",
  components: {
    HelloWorld,
    InformationFlex,
    Faq,
    Events,
    Footer,
  },
};
</script>
