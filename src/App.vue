<template>
  <div id="app">
   
   <Header />


  <main>
    <div class="container">
      <DatesComponent />
      <AboutMeComponent />
      <CoursesComponent />

      
     
    </div>
    <!-- /.container -->
  </main>

  </div>
</template>

<script>
import Header from '@/components/SiteHeader.vue'
import DatesComponent from '@/components/DatesSectionComponent.vue'
import AboutMeComponent from '@/components/AboutMeSectionComponent.vue'
import CoursesComponent from '@/components/CoursesSectionComponent.vue'
export default {
  name: 'App',
  components: {
    Header,
    DatesComponent,
    AboutMeComponent,
    CoursesComponent,
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

main {
 
}

</style>
