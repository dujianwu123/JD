<template lang="html">
    <div>
      <Heador></Heador>
      <Mslider></Mslider>
      <Ada></Ada>
      <Money></Money>
      <Adb></Adb>
      <Finance></Finance>
      <Adc></Adc>
      <Footor cname="mfooter"></Footor>
      <Navbar></Navbar>
    </div>
</template>

<script>
import Heador from "../public/header";
import Footor from "../public/footer.vue";
import Navbar from "../public/navbar.vue";
import Mslider from "./mslider";
import Ada from "./ada";
import Adb from "./adb";
import Money from "./money";
import Finance from "./finance";
import Adc from "./adc";
export default {
  components: {
    Heador,
    Footor,
    Navbar,
    Mslider,
    Ada,
    Adb,
    Money,
    Finance,
    Adc
  }
};
</script>

<style lang="scss">
.mfooter {
  margin-top: 0 !important;
  ul {
    li:first-child {
      display: none;
    }
  }
}
</style>

