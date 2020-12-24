<template>
  <div>
    <PromoBar message="FREE SHIPPING ON ALL ORDERS OVER $75"></PromoBar>
    <Header></Header>
    <Hero></Hero>
    <Categories></Categories>
    <Arrivals> </Arrivals>
    <CTA :ctaBgImage="ctaImage"> </CTA>
    <Instagram></Instagram>
    <Newsletter></Newsletter>
    <Footer></Footer>
  </div>
</template>

<script>
import Vue from "vue";
import Header from "./components/Header.vue";
import Footer from "./components/Footer.vue";
import PromoBar from "./components/PromoBar.vue";
import Hero from "./components/Hero.vue";
import Categories from "./components/Categories.vue";
import Arrivals from "./components/Arrivals.vue";
import CTA from "./components/CTA.vue";
import Instagram from "./components/Instagram.vue";
import Newsletter from "./components/Newsletter.vue";

export default Vue.extend({
  name: "App",
  data() {
    return {
      ctaImage: require('./assets/images/cta-background-image.jpg')
    };
  },
  components: {
    Header,
    Footer,
    PromoBar,
    Hero,
    Categories,
    Arrivals,
    CTA,
    Instagram,
    Newsletter
  },
});
</script>