<template>
  <header>
     <div class="container">
       <Navbar />
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