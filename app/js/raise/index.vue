<template lang="html">
    <div>
      <Heador></Heador>
      <Rslider></Rslider>
      <Footor cname="mfooter"></Footor>
      <Navbar></Navbar>
    </div>
</template>

<script>
import Heador from "../public/header";
import Footor from "../public/footer.vue";
import Navbar from "../public/navbar.vue";
import Rslider from "./rslider";
export default {
  components: {
    Heador,
    Footor,
    Navbar,
    Rslider
  }
};
</script>

<style lang="scss">
@import "../../css/reset.scss";
.mfooter {
  margin-top: 0 !important;
  ul {
    li:first-child {
      display: none;
    }
  }
}
</style>

