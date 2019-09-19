<template>
  <div class="content">
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
          href: "ious",
          src:
            "//img12.360buyimg.com/jrpmobile/jfs/t8491/303/504628479/60643/100648de/59a94358N92475fca.jpg?width=750&height=320"
        },
        {
          href: "home",
          src:
            "//img12.360buyimg.com/jrpmobile/jfs/t8437/321/1758527686/40952/f66d552f/59bf1f41N50d846f9.jpg?width=750&height=320"
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