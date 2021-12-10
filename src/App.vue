<template>
  <div id="app">
    <!-- HEADER -->
    <Header />
    <!-- MAIN -->
    <Main />

    <!-- FOOTER -->
    <Footer />
  </div>
</template>

<script>
import Header from '@/components/Header.vue'
import Main from '@/components/Main.vue'
import Footer from '@/components/Footer.vue'


export default {
  name: 'App',
  components: {
    Header,
    Main,
    Footer,
  }
}
</script>

<style lang="scss">
  .site-btn {
    border: 1px solid #ae8652;
    color: #ae8652;
    background: none;
    text-transform: uppercase;
    padding: 5px 16px;
  }

  h1,h2,h3,h4,h5,h6 {
    font-family: 'Playfair Display', serif;
    font-weight: 700 !important;
  }
</style>
