<template>
  <footer id="footer" class="footer">
    <div class="footer-inner">
      <div class="menu-1">
        <span class="label">Customer Service
          <span class="toggler">-</span>
        </span>
        <ul>
          <li>Accessibility</li>
          <li>Contact Us</li>
          <li>Return Policy</li>
          <li>FAQ</li>
          <li>Gift Certificates</li>
          <li>Wishlist</li>
          <li>About Us</li>
        </ul>
      </div>
      <div class="menu-2">
        <span class="label">Company
            <span class="toggler">+</span>
        </span>
        <ul>
          <li>About Us</li>
          <li>Careers</li>
          <li>Press</li>
          <li>Affiliates</li>
        </ul>
      </div>
      <div class="menu-3">
        <span class="label">Follow Us</span>
        <ul>
          <li v-for="(image, index) in socialImages" :key="index">
            <img :src="image" alt="social-icon" />
          </li>
        </ul>
      </div>
    </div>
  </footer>
</template>

<script>
import $ from 'jquery';

export default {
  mounted: function () {
    $('.toggler').on('click', function(event) {
      if ($(event.currentTarget).html() == '+') {
        $(event.currentTarget).parent().next().slideDown();
        $(event.currentTarget).html('-');
      } else {
        $(event.currentTarget).parent().next().slideUp();
        $(event.currentTarget).html('+');
      }
    })
  },
  data: function() {
    return {
      socialImages: [
        require("../assets/images/facebook-icon.png"),
        require("../assets/images/instagram-icon.png"),
        require("../assets/images/twitter-icon.png"),
      ] 
    }
  }
};
</script>

<style>
</style>