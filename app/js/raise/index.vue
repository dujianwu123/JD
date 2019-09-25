<template lang="html">
    <div>
      <Heador></Heador>
      <Rslider></Rslider>
      <Daily></Daily>
      <In></In>
      <More></More>
      <Footor cname="mfooter"></Footor>
      <Navbar></Navbar>
    </div>
</template>

<script>
import Heador from "../public/header";
import Footor from "../public/footer.vue";
import Navbar from "../public/navbar.vue";
import Rslider from "./rslider";
import Daily from './daily';
import In from './in';
import More from './more';
export default {
  components: {
    Heador,
    Footor,
    Navbar,
    Rslider,
    Daily,
    In,
    More
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

