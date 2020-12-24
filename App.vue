<template>
<div>
    <PromoBar message="FREE SHIPPING ON ALL ORDERS OVER $75"></PromoBar>
    <Header compName="header"></Header>
    <!-- <Hero /> -->
    <Categories />
    <Arrivals />
</div>
</template>

<script>
import Vue from "vue";
import Header from './components/Header.vue'
import Footer from './components/Footer.vue'
import PromoBar from './components/PromoBar.vue'
import Hero from './components/Hero.vue'
import Categories from './components/Categories.vue'
import Arrivals from './components/Arrivals.vue'

export default Vue.extend({
  name: 'App',
  data() {
    return {
    };
  },
  components: {
    Header,
    Footer,
    PromoBar,
    Hero,
    Categories,
    Arrivals
  }
});
</script>

<style lang="scss" scoped>

</style>