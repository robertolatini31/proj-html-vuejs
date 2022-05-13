<template>
  <div id="app">
   
   <header>
     <div class="container">
       <nav class="d-flex justify-content-between">
       <div class="logo">
         <img src="@/assets/img/dark-logo.png" alt="logo">
       </div>
       <!-- /.logo -->
       <div class="menu">
         <ul class="d-flex">
            <li class="d-flex align-items-center" v-for="link in HeaderMenu" :key="link">
             <a href="#">{{link}}</a>
             <font-awesome-icon class="icon_arrow_down" icon="fa-solid fa-angle-down" />
            </li>
         </ul>
       </div>
       <!-- /.menu -->
       <div class="social_nav">

          <font-awesome-icon class="icon_social_nav" icon="fa-brands fa-twitter" />
          <font-awesome-icon class="icon_social_nav" icon="fa-brands fa-facebook-f" />
          <font-awesome-icon class="icon_social_nav" icon="fa-brands fa-instagram" />
          <font-awesome-icon class="icon_social_nav" icon="fa-brands fa-linkedin" />

       </div>
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
    
  },
  data () {
    return {
      HeaderMenu: [
        'Home',
        'Pages',
        'Courses',
        'Features',
        'Blog',
        'Shop',
      ]
    }
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
    .menu {
      ul {
        list-style: none;
        margin: 0;
        padding: 0;
        column-gap: 3rem;
        li {
          a {
            text-decoration: none;
            color: black;
            padding-right: 0.3rem;
          }
          .icon_arrow_down {
            font-size: 0.6rem;
          }
        }
      }
    }
    .social_nav {
      .icon_social_nav {
        margin-right: 1rem;
        font-size: 1.2rem;
      }
    }
  }
}
}
</style>
