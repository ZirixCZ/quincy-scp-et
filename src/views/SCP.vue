<template>
  <div class="SCP">
    <PictureSCP title="" />
  </div>
</template>

<script>
// @ is an alias to /src
import PictureSCP from "@/components/PictureSCP.vue";

export default {
  name: "Home",
  components: {
      PictureSCP,
  },
};
</script>
<style scoped lang="scss">
.SCP {
    background-color: #080908;
    height: 1000vh;
}
@media only screen and (min-device-width: 320px) and (max-device-width: 480px) {
  .SCP {
    height: 3000vh;
  }
}
</style>