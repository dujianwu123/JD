<template>
  <section :class="cname">
    <swiper :options="options" :not-next-tick="options.notNextTick">
      <swiper-slide v-for="item in items" :key="item.href">
        <router-link :to="{ name: item.href }">
          <img :src="item.src" />
        </router-link>
      </swiper-slide>
      <div class="swiper-pagination" v-if="options.pagination" slot="pagination"></div>
    </swiper>
  </section>
</template>

<script>
import { swiper, swiperSlide } from "vue-awesome-swiper";
export default {
  components: {
    swiper,
    swiperSlide
  },
  props: {
    cname: {
      type: String,
      default: ""
    },
    options: {
      type: Object,
      default: function() {
        return {
          autoplay: true,
          loop: true, // 循环比如拉到最后一张在拉会自动是第一张
          pagination: {
            el: ".swiper-pagination"
          },
          notNextTick: false
        };
      }
    },
    items: {
      type: Array,
      default() {
        return [];
      }
    }
  },
  data() {
    return {};
  }
};
</script>

<style lang="scss">
@import "~swiper/dist/css/swiper.css";

</style>