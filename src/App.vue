<template>
  <div id="app">
   
   <div class="fixed_menu d-flex flex-column">
     <font-awesome-icon class="fixed_icon" icon="fa-solid fa-ruler-combined" />
     <font-awesome-icon class="fixed_icon" icon="fa-solid fa-life-ring" />
     <font-awesome-icon class="fixed_icon" icon="fa-solid fa-book" />
     <font-awesome-icon class="fixed_icon" icon="fa-solid fa-cart-shopping" />
   </div>
   <!-- /.fixed_menu -->


  <Header />
  <Main />
  <Footer />
  
  </div>
</template>

<script>
import Header from '@/components/SiteHeader.vue'
import Main from '@/components/SiteMain.vue'
import Footer from '@/components/SiteFooter.vue'
export default {
  name: 'App',
  components: {
    Header,
    Main,
    Footer,
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


.fixed_menu {
  z-index: 10000;
  position: fixed;
  top: 130px;
  right: -5px;
  border-radius: 5px;
  background-color: white;
  box-shadow: 0 0 8px -4px black;
  .fixed_icon:hover {
    color: $Primary-color;
  }
  .fixed_icon {
    padding: 0.8rem;
    font-size: 1rem;
    cursor: pointer;
  }
}


</style>
