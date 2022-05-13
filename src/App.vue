<template>
  <div id="app">
   
   <header>
     <div class="container">
       <nav class="d-flex justify-content-between">
       <div class="logo">
         <img src="@/assets/img/dark-logo.png" alt="logo">
       </div>
       <!-- /.logo -->
       <div class="menu">MENU</div>
       <!-- /.menu -->
       <div class="social_nav">SOCIAL</div>
       <!-- /.social_nav -->
      </nav>
     </div>
     <!-- /.container -->
   </header>


  </div>
</template>

<script>

export default {
  name: 'App',
  components: {
    
  }
}
</script>

<style lang="scss">
@import '@/assets/scss/style.scss';


#app {
header {
  nav {
    padding: 1rem 0;
    .logo {
      img {
        max-width: 150px;
      }
    }
  }
}
}
</style>
