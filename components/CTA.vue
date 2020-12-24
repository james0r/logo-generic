<template>
  <section id="cta-section" class="cta-section">
    <div class="cta-section-inner"     
        v-bind:style="{
          backgroundImage: 'url(' + ctaBgImage + ')',
        }">

    <div class="content">
      <h2>
        Title Goes Here
      </h2>
      <h4>
        Tagline goes right here.
      </h4>
      <a href="/">
        SHOP NOW
      </a>
    </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'CTA',
  props: ['ctaBgImage']
}
</script>

<style>

</style>