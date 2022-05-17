<template>
  <div id="app">
  <FixedMenu />
  <Header />
  <Main />
  <Footer />
  </div>
</template>

<script>
import Header from '@/components/SiteHeader.vue'
import Main from '@/components/SiteMain.vue'
import Footer from '@/components/SiteFooter.vue'
import FixedMenu from '@/components/FixedMenuComponent.vue'
export default {
  name: 'App',
  components: {
    Header,
    Main,
    Footer,
    FixedMenu,
  },
  
  
}
</script>

<style lang="scss">
@import '@/assets/scss/style.scss';
@import url('https://fonts.googleapis.com/css2?family=Playfair+Display&display=swap');

#app {
  color: $Dark-color;
}

.title {
  font-family: 'Playfair Display', serif;
}

.py_4 {
  padding: 4rem 0;
}

</style>
