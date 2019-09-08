<template lang="html">
    <div>
      <Heador></Heador>
      <Hslider></Hslider>
      <Novie></Novie>
      <Borrow></Borrow>
      <Money></Money>
      <Product></Product>
      <Life></Life>
      <Footor></Footor>
      <Navbar></Navbar>
    </div>
</template>

<script>
import Heador from '../public/header';
import Footor from "../public/footer.vue"
import Navbar from "../public/navbar.vue"
import Hslider from './hslider';
import Novie from './novice';
import Borrow from './borrow';
import Money from './money';
import Product from './product';
import Life from './life';

export default {
  components: {
    Heador,
    Hslider,
    Novie,
    Borrow,
    Money,
    Product,
    Life,
    Footor,
    Navbar
  }
}
</script>

<style lang="scss" module>
  @import '../../css/reset.scss';
  .home{
    color: red;
    font-size: 80px;
  }
</style>
