<template>
   <main>
    <div class="container">
      <DatesComponent />
      <AboutMeComponent />
      <CoursesComponent />
      <BooksComponent />
    </div>
    <!-- /.container -->
    <TestimonialsComponent />
    <div class="container">
      <BlogUpdatedComponent />
    </div>
    <!-- /.container -->
  </main>
</template>

<script>
import DatesComponent from '@/components/DatesSectionComponent.vue'
import AboutMeComponent from '@/components/AboutMeSectionComponent.vue'
import CoursesComponent from '@/components/CoursesSectionComponent.vue'
import BooksComponent from '@/components/BooksSectionComponent.vue'
import TestimonialsComponent from '@/components/TestimonialsSectionComponent.vue'
import BlogUpdatedComponent from '@/components/BlogUpdatedSectionComponent.vue'
export default {
name: 'SiteMain',
components: {
    DatesComponent,
    AboutMeComponent,
    CoursesComponent,
    BooksComponent,
    TestimonialsComponent,
    BlogUpdatedComponent,
}
}
</script>

<style>

</style>