<template>
  <header>
     <div class="container">
       <Navbar :HeaderMenu="HeaderMenu"/>
      <HeroImage />
     </div>
     <!-- /.container -->
   </header>
</template>

<script>
import Navbar from '@/components/NavbarComponent.vue'
import HeroImage from '@/components/HeroImageComponent.vue'
export default {
name: 'SiteHeader',
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
      ],
    }
  },
components: {
  Navbar,
  HeroImage,
}
}
</script>

<style lang="scss" scoped>
header {
  background-image: url('@/assets/img/background-pattern-wavify.png');
  background-color: $Light-bg-color;
}
</style>