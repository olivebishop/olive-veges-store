<script setup>
import '../assets/styles/Home.scss'
import HeaderText from '../components/HeaderText.vue'
import HomeProduct from '../components/HomeProduct.vue';
</script>

<template>
  <main>
    <section class="home bg-blue">
      <HeaderText />
      <img src="@/assets/images/landing.png" alt="Sneaker" id="headerImg">
    </section>
    <section class="products">
      <HomeProduct />
    </section>
  </main>
  <footer class="footer">
    <hr>
    <a class="a"  href="https://luqmanshaban.com" target="_blank">Created by Luqman Shaban</a>
    <p class="text-orange-600">&copy; All rights reserved</p>
  </footer>
</template>

