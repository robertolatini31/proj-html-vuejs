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
          <font-awesome-icon class="icon_social_nav change_menu" icon="fa-solid fa-bars" />
          <font-awesome-icon class="icon_social_nav d_none_sm" icon="fa-brands fa-twitter" />
          <font-awesome-icon class="icon_social_nav d_none_sm" icon="fa-brands fa-facebook-f" />
          <font-awesome-icon class="icon_social_nav d_none_sm" icon="fa-brands fa-instagram" />
          <font-awesome-icon class="icon_social_nav d_none_sm" icon="fa-brands fa-linkedin" />

       </div>
       <!-- /.social_nav -->
      </nav>
      <!-- /.nav  -->
      <div class="hero_image pt-5">
        <div class="row row-cols-2">
          <div class="col d-flex">
             <div class="hero_text align-self-center">
                <span class="text-uppercase">i'm wingman</span>
              <h1 class="title pb-4 m-0 pt-4 text-capitalize">peace on earth a <br> wonderful wish <br> but no way</h1>
              <p class="m-0 pb-4">Success isn't overnight. It's when everyday you get a little <br> better than day before. it all adds up.</p>
              <button>
                <div class="button_text d-flex">
                  <span class="text-capitalize me-2">get started for free</span>
                  <font-awesome-icon class="align-self-center" icon="fa-solid fa-arrow-right-long" />
                </div>
              </button>
             </div>
             <!-- /.hero_text -->
          </div>
          <!-- /.col -->
          <div class="col col_hero_img">
            <img src="@/assets/img/home-movation-hero-image.png" alt="hero_image">
          </div>
          <!-- /.col -->
        </div>
        <!-- /.row -->
      </div>
      <!-- /.hero_image -->
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
@import url('https://fonts.googleapis.com/css2?family=Playfair+Display&display=swap');

.title {
  font-family: 'Playfair Display', serif;
}
#app {
header {
  background-image: url('@/assets/img/background-pattern-wavify.png');
  background-color: #F7F7FD;

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
          a, .icon_arrow_down {
            color: $Secondary-color;
          }
          a {
            text-decoration: none;
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
        color: $Dark-color;
      }
      .change_menu {
        display: none;
      }    
    }
  }
}
@media screen and (max-width:"992px") {
  .menu {display: none;}
  .change_menu {
    display: inline-block!important;
  }
}
@media screen and (max-width:"576px") {
  .d_none_sm {
    display: none;
  }
}

.hero_image {
  .hero_text {
    color: $Dark-color;
    span, p, .button_text {
      font-size: 0.8rem;
    }
    span {
    font-weight: 500;
    }
    p {
      color: $Light-Dark-color;
    }
    button {
      border: none;
      border-radius: 5px;
      background-color: $Primary-color;
      .button_text {
        color: white;
        padding: 0.8rem 2.5rem;
      }
    }
  }

  .col_hero_img {
    background-image: url('@/assets/img/home-movation-shape-face.png');
    background-repeat: no-repeat;
    background-position: bottom;
    background-size: 450px;
    img {
      height: 500px;
    }
  }
  
}

}
</style>
