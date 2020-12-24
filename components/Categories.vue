<template>
  <section id="categories" class="categories">
    <div class="categories-inner">
      <ul class="flex category-list">
        <li v-for="(item, index) in items" :key="index" class="category-item">
          <img :src="item.image" :alt="item.alt">
          <div class="cat-item-label">
            {{ item.title }}
          </div>
        </li>
      </ul>
    </div>
  </section>
</template>

<script>
export default {
  name: 'Categories',
  data: function() {
    return {
      items: [
        {
          image: require('../assets/images/cat-image-womens.jpg'),
          title: 'Womens',
          alt: 'womens clothing',
          link: '/'
        },
        {
          image: require('../assets/images/cat-image-mens.jpg'),
          title: 'Mens',
          alt: 'mens clothing',
          link: '/'
        },
        {
          image: require('../assets/images/cat-image-accessories.jpg'),
          title: 'Accessories',
          alt: 'clothing accessories',
          link: '/'
        }
      ]
    }
  }
}
</script>

<style>

</style>