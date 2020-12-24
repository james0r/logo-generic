<template>
  <section id="categories" class="categories">
    <div class="categories-inner">
      <ul class="flex category-list">
        <li v-for="(item, index) in items" :key="index" class="category-item">

        </li>
      </ul>
    </div>
  </section>
</template>

<script>
export default {
  data: function() {
    return {
      items: [
        {
          image: require('../assets/images/cat-image-womens.jpg'),
          title: 'Womens',
          link: '/'
        },
        {
          image: require('../assets/images/cat-image-mens.jpg'),
          title: 'Mens',
          link: '/'
        },
        {
          image: require('../assets/images/cat-image-accessories.jpg'),
          title: 'Accessories',
          link: '/'
        }
      ]
    }
  }
}
</script>

<style>

</style>