<template>
  <section id="arrivals" class="arrivals">
    <div class="arrivals-inner">
      <VueSlickCarousel class="arrivals-list">
        <li v-for="(item, index) in items" :key="index" class="category-item">
          <img :src="item.image" :alt="item.alt">
          <div class="cat-item-label">
            {{ item.title }}
          </div>
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
  name: 'Arrivals',
  components: {
    VueSlickCarousel
  },
  data: function() {
    return {
      items: [
        {
          image: require('../assets/images/cat-image-womens.jpg'),
          title: 'Product Title',
          alt: 'womens clothing',
          link: '/',
          price: ''
        }
      ]
    }
  }
}
</script>

<style>

</style>