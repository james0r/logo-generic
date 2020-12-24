<template>
  <section id="arrivals" class="arrivals">
    <div class="arrivals-inner">
      <div class="section-title">
        <span>New Arrivals</span>
      </div>
      <VueSlickCarousel class="arrivals-list" v-bind="settings">
        <template #prevArrow="arrowOption">
          <div class="arrivals-left-arrow">
            <img :src="arrowRight" alt="previous slide arrow" />
            {{ arrowOption.currentSlide }}/{{ arrowOption.slideCount }}
          </div>
        </template>
        <template #nextArrow="arrowOption">
          <div class="arrivals-right-arrow">
            <img :src="arrowRight" alt="next slide arrow" />
            {{ arrowOption.currentSlide }}/{{ arrowOption.slideCount }}
          </div>
        </template>

        <li v-for="(item, index) in 8" :key="index" class="arrivals-item">
          <a href="/">
            <div class="prod-image image-wrapper">
              <img :src="image" :alt="item.alt" />
            </div>
            <h4 class="prod-title">Product Title</h4>
            <div class="prod-description">Women's T-Shirt</div>
            <div class="prod-price">$19.99</div>
          </a>
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

export default {
  name: "Arrivals",
  components: {
    VueSlickCarousel,
  },
  data: function () {
    return {
      arrowRight: require("../assets/images/arrow-right.png"),
      settings: {
        dots: false,
        infinite: false,
        speed: 500,
        slidesToShow: 4,
        slidesToScroll: 1,
        initialSlide: 0,
        responsive: [
          {
            breakpoint: 1024,
            settings: {
              slidesToShow: 3,
              slidesToScroll: 1,
              infinite: true,
              dots: false,
            },
          },
          {
            breakpoint: 600,
            settings: {
              slidesToShow: 2,
              slidesToScroll: 1,
              initialSlide: 1,
            },
          },
          {
            breakpoint: 374,
            settings: {
              slidesToShow: 1,
              slidesToScroll: 1,
            },
          },
        ],
      },
      image: require("../assets/images/arrivals-product-image.jpg"),
    };
  },
};
</script>

<style>
</style>