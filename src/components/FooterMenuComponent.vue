<template>
   <div class="footer_info py_4">
        <div class="row row-cols-1 row-cols-lg-2">
          <div class="col address_col pb-4">
            <h5>Address</h5>
            <ul class="p-0 m-0">
              <li>
                <a href="#">382 NE 191st St # 87394 Miami, FL 33179-3899</a>
              </li>
              <li>
                <a href="#">+1 (305) 547-9909 (9am - 5pm EST, Monday - Friday)</a>
              </li>
              <li>
                <a href="#">support@maxcoach.com</a>
              </li>
            </ul>
            <div class="footer_social pt-3">
              <a href="#" class="social_icon me-3"><font-awesome-icon icon="fa-brands fa-facebook-square" /></a>
              <a href="#" class="social_icon me-3"><font-awesome-icon icon="fa-brands fa-twitter" /></a>
              <a href="#" class="social_icon me-3"><font-awesome-icon icon="fa-brands fa-instagram" /></a>
              <a href="#" class="social_icon"><font-awesome-icon icon="fa-brands fa-linkedin" /></a>
            </div>
          </div>
          <!-- /.col -->
          <div class="col menu_col pt-4">
            <div class="row row-cols-2 row-cols-sm-3">
              <div class="col mb-4" v-for="(MenuItem, index) in MenuItems" :key="MenuItem.name + index">
                <h5>{{MenuItem.name}}</h5>
                <ul class="p-0 m-0">
                  <li v-for="link in MenuItem.links" :key="link">
                    <a href="#">{{link}}</a>
                  </li>
                </ul>
              </div>
              <!-- /.col -->
            </div>
            <!-- /.row -->
          </div>
          <!-- /.col -->
        </div>
        <!-- /.row -->
      </div>
      <!-- /.footer_info -->
</template>

<script>
export default {
name: 'FooterMenuComponent',
props: {
    MenuItems: Array,
}
}
</script>

<style lang="scss" scoped>
 .footer_info {
    
      h5 {
        color: white;
        min-height: 24px;
      }
      ul {
        list-style: none;
        li {
           
          padding: 0.8rem 0;
          a {
               transition: all .2s;
            text-decoration: none;
            color: $Light-Dark-color;
            font-size: 0.8rem;
          }
        }
        li:hover {
          a {
            color: $Primary-color;
          }
        }
      }
      .footer_social {
        .social_icon {
            transition: all .2s;
            text-decoration: none;
             color: $Light-Dark-color;
             font-size: 1.5rem;
        }
        .social_icon:hover {
          color: white;
        }
      }
    }
</style>