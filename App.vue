<template>
<div>
    <PromoBar message="FREE SHIPPING ON ALL ORDERS OVER $75"></PromoBar>
    <Header compName="header"></Header>
    <Hero />
    <Categories />
</div>
</template>

<script>
import Vue from "vue";
import Header from './components/Header.vue'
import Footer from './components/Footer.vue'
import PromoBar from './components/PromoBar.vue'
import Hero from './components/Hero.vue'
import Categories from './components/Categories.vue'

export default Vue.extend({
  data() {
    return {
      bundler: "Parcel"
    };
  },
  components: {
    Header,
    Footer,
    PromoBar,
    Hero,
    Categories
  }
});
</script>

<style lang="scss" scoped>

</style>