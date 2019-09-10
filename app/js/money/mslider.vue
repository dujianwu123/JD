<template>
  <div>
    <Slider :items="items" cname="slider"></Slider>
  </div>
</template>

<script>
import Slider from "../core/slider";
export default {
  data() {
    return {
      items: [
        {
          href: "home",
          src:
            "//img12.360buyimg.com/jrpmobile/jfs/t11149/181/856008463/68797/dc303e9/59f97baeN3cdae084.jpg?width=750&height=400"
        },
        {
          href: "home",
          src:
            "//img12.360buyimg.com/jrpmobile/jfs/t9994/205/2575467053/189117/125e7b05/59f97c36N7599be57.png?width=750&height=400"
        }
      ]
    };
  },
  components: {
    Slider
  }
};
</script>
<style lang="scss">
.slider {
  margin-top: 120px;
  img {
    width: 100%;
  }
  .swiper-pagination-bullet {
    box-sizing: border-box;
    border-radius: 7px;
    height: 3px;
    width: 8px;
    background: rgba(248, 241, 241, 0.4);
    margin: 0 2px;
    display: inline-block;
    opacity: 1;
  }
  .swiper-pagination-bullet-active {
    background: #c7c1c1;
    width: 12px;
  }
}
</style>
<style lang="scss" module>
@import "../../css/reset.scss";
</style>