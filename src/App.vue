<template>
  <div id="app">
   
   <Header />


  </div>
</template>

<script>
import Header from '@/components/SiteHeader.vue'
export default {
  name: 'App',
  components: {
    Header,
  },
  
}
</script>

<style lang="scss">
@import '@/assets/scss/style.scss';
@import url('https://fonts.googleapis.com/css2?family=Playfair+Display&display=swap');


.title {
  font-family: 'Playfair Display', serif;
}

</style>
