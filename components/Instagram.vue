<template>
  <section id="instagram" class="instagram">
    <div class="instagram-inner">
      <div class="section-title">
        Follow us on Instagram!
      </div>
      <ul class="image-list">
        <li v-for="(image, index) in images" :key="index">
          <img class="instagram-image" :src="image" alt="instagram image">
        </li>
      </ul>
    </div>
  </section>
</template>

<script>
export default {
  name: 'Instagram',
  data: function() {
    return {
      images: [
        require('../assets/images/insta-1.jpg'),
        require('../assets/images/insta-2.jpg'),
        require('../assets/images/insta-3.jpg'),
        require('../assets/images/insta-4.jpg'),
        require('../assets/images/insta-5.jpg'),
      ]
    }
  }
}
</script>

<style>

</style>