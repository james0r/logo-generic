<template>
  <section id="home-hero" class="home-hero">
    <div class="home-hero-inner">
      <VueSlickCarousel :arrows="true" :dots="true" class="mobile-slider">
        <li v-for="item in 4" :key="item">
          <MobileSlide
            :bgImage="mobileBgImage"
            btnText="SHOP NOW"
            btnLink="/"
            title="Title Goes Here"
            tagline="Tagline will go right here."
          />
        </li>
      </VueSlickCarousel>
      <VueSlickCarousel :arrows="true" :dots="true" class="desktop-slider">
        <li v-for="item in 4" :key="item">
          <DesktopSlide
            :bgImage="desktopBgImage"
            btnText="SHOP NOW"
            btnLink="/"
            title="Title Goes Here"
            tagline="Tagline will go right here."
          />
        </li>
      </VueSlickCarousel>
    </div>
  </section>
</template>

<script>
import VueSlickCarousel from "vue-slick-carousel";
import "vue-slick-carousel/dist/vue-slick-carousel.css";
// optional style for arrows & dots
import "vue-slick-carousel/dist/vue-slick-carousel-theme.css";
import MobileSlide from "./MobileSlide";
import DesktopSlide from "./DesktopSlide";

export default {
  mounted: function () {},
  components: { VueSlickCarousel, MobileSlide, DesktopSlide },
  data: () => {
    return {
      mobileBgImage: require("../assets/images/slide-bg-mobile.jpg"),
      desktopBgImage: require("../assets/images/slide-bg-desktop.jpg"),
    };
  },
};
</script>

<style>
</style>