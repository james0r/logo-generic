<template>
  <section id="newsletter" class="newsletter">
    <div class="newsletter-inner">
      <img :src="icon" alt="decorative image" class="newsletter-icon" />
      <h2>Sign up & Stay connected</h2>
     <div class="description-n-form">
        <div class="newsletter-details">
          <p>
            Sign up for the newsletter and get 20% off! Get access to exclusive
            offers and be the first to know when new stuff drops.
          </p>
        </div>
        <form action="/" class="newsletter-form">
          <input type="email" placeholder="Your Email Address">
          <input type="submit" value="Subscribe" tabindex="0">
        </form>
     </div>
    </div>
  </section>
</template>

<script>
export default {
  data: function () {
    return {
      icon: require("../assets/images/newsletter-icon.png"),
    };
  },
};
</script>

<style>
</style>