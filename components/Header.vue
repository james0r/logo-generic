<template>
  <header id="header" class="header">
    <div class="header-inner flex">
      <img class="mobile-menu-icon" aria-role="button" src="../assets/images/hamburger-icon.png" alt="hamburger icon" tabindex="0">
      <a href="/">
        <img src="../assets/images/logo-mobile.png" alt="company logo" class="header-logo-mobile">
      </a>
      <ul id="primary-menu" class="primary-menu">
        <li>Womens</li>
        <li>Mens</li>
        <li>Accessories</li>
        <li>Sale</li>
      </ul>
      <img class="cart-icon" aria-role="button" src="../assets/images/cart-icon.png" alt="shopping cart" tabindex="0">
    </div>
  </header>
</template>

<script>
export default {
  name: 'Header',
  props: ['compName']
}
</script>

<style>

</style>