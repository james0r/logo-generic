<template>
  <div
    class="slide-inner"
    v-bind:style="{
      backgroundImage: 'url(' + bgImage + ')',
    }"
  >
    <div class="content">
      <h2 class="slide-title">
        {{ title }}
      </h2>
      <h4>
        {{ tagline }}
      </h4>
      <a :href="btnLink" class="btn">
        {{ btnText }}
      </a>
    </div>
  </div>
</template>

<script>
export default {
  name: 'DesktopSlide',
  props: ["title", "tagline", "btnText", "btnLink", "bgImage"],
};
</script>

<style>
</style>