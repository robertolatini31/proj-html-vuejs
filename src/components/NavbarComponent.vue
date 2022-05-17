<template>
  <nav class="d-flex justify-content-between py-4">
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

        <div class="drop_container">
            <font-awesome-icon @click="DropToggle" class="icon_social_nav change_menu" icon="fa-solid fa-bars" />

            <div @mouseleave="DropOff" :class="ControlDrop ? 'd_show' : ''" class="change_menu_drop p-3 border">
                    <ul class="d-flex flex-column p-0 m-0">
                    <li class="d-flex align-items-center py-2" v-for="HeaderMenuItem in HeaderMenu" :key="HeaderMenuItem.name">
                    
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
        </div>
        <!-- /.drop_container -->
        


          
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
props: {
    HeaderMenu: Array,
},
data () {
    return {
        ControlDrop: false,
    }
},
  methods: {
      DropToggle() {
          if (this.ControlDrop == false) {
              this.ControlDrop = true;
          } else {
               this.ControlDrop = false;
          }
      },
      DropOff() {
          this.ControlDrop = false;
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
              transition: all .2s;
            color: $Secondary-color;
          }
          a {
              transition: all .5s;
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
          transition: all .2s;
        cursor: pointer;
        margin-right: 1rem;
        font-size: 1.2rem;
        color: $Dark-color;
      }
      .change_menu {
          display: none;
      }
      .d_show {
          display: block!important;
      }
      .change_menu_drop {
        background-color: white;
        
        display: none;
        position: absolute;
        top: 1.2rem;
        right: 0;
        border-radius: 5px;
      }    
      .drop_container {
          display: inline-block;
          position: relative;
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