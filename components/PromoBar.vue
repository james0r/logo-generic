<template>
  <section id="promo-bar" class="promo-bar">
    <div class="promo-bar-inner">
      <span class="promo-bar-message">{{ message }}</span>
    </div>
  </section>
</template>

<script>
export default {
  name: 'PromoBar',
  props: ['message']
}
</script>

<style>

</style>