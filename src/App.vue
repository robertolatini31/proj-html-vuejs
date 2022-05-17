<template>
  <div id="app">
   
   <Header />
   <Main />
  
  <footer>

    

  </footer>

  </div>
</template>

<script>
import Header from '@/components/SiteHeader.vue'
import Main from '@/components/SiteMain.vue'
export default {
  name: 'App',
  components: {
    Header,
    Main,
  },
  
}
</script>

<style lang="scss">
@import '@/assets/scss/style.scss';
@import url('https://fonts.googleapis.com/css2?family=Playfair+Display&display=swap');


.title {
  font-family: 'Playfair Display', serif;
}

.py_4 {
  padding: 4rem 0;
}


</style>
