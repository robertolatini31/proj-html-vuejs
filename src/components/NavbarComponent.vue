<template>
  <nav class="d-flex justify-content-between">
       <div class="logo">
         <img src="@/assets/img/dark-logo.png" alt="logo">
       </div>
       <!-- /.logo -->
       <div class="menu">
         <ul class="d-flex">
            <li class="d-flex align-items-center" v-for="HeaderMenuItem in HeaderMenu" :key="HeaderMenuItem.name">
             
                <div class="dropdown">
                    <a class="dropdown-toggle" href="#" data-bs-toggle="dropdown" aria-expanded="false">
                        {{HeaderMenuItem.name}}
                        <font-awesome-icon class="icon_arrow_down" icon="fa-solid fa-angle-down" />
                    </a>

                    <ul class="dropdown-menu">
                        <li v-for="link in HeaderMenuItem.links" :key="link">
                            <a class="dropdown-item" href="#">{{link}}</a>
                        </li>
                    </ul>
                </div>

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
</template>

<script>
export default {
name: 'NavbarComponent',
data () {
    return {
      HeaderMenu: [
          {
              name: 'Home',
              links: [
                  'MaxCoach Education',
                  'Course Portal',
                  'Distant Learning',
                  'Multimedia Pedagogy',
              ],
          },
          {
              name: 'Pages',
              links: [
                  'Start Here',
                  'Success Story',
                  'About Me',
              ],
          },
          {
              name: 'Courses',
              links: [
                  'Courses Grid 01',
                  'Courses Grid 02',
                 'Courses Grid 03',
              ],
          },
           {
              name: 'Features',
              links: [
                  'Events',
                  'Zoom Meetings',
              ],
          },
            {
              name: 'Blog',
              links: [
                  'Blog Grid',
                  'Blog Classic',
              ],
          },
          {
              name:  'Shop',
              links: [
                  'Shop Left Sidebar',
                  'Shop Right Sidebar',
                  'Cart',
                  'Wishlist'
              ],
          },
        
        
        
        
        
       
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
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
        li:hover a, li:hover .icon_arrow_down {
            color: $Primary-color;
        }
        li {
          a, .icon_arrow_down {
            color: $Secondary-color;
          }
          a {
            text-decoration: none;
            padding-right: 0.3rem;
          }
          .icon_arrow_down {
            font-size: 0.7rem;
          }
          .dropdown-toggle::after {
              content: none;
          } 
          .dropdown-menu > li > a:hover {
                background-image: none;
                background-color: $Primary-color;
                color: white;
            }
        }
      }
    }
    .social_nav {
        .icon_social_nav:hover {
            color: $Primary-color;
        }
      .icon_social_nav {
        cursor: pointer;
        margin-right: 1rem;
        font-size: 1.2rem;
        color: $Dark-color;
      }
      .change_menu {
        display: none;
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
</style>