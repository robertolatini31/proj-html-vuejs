<template>
  <footer>
    <div class="container">
     <FooterMenu />
      <h6 class="text-center py_4 m-0">&copy; 2020 Maxcoach. All Rights Reserved</h6>
    </div>
    <!-- /.container -->
   <GoUp />
  </footer>

</template>

<script>
import GoUp from '@/components/GoUpComponent.vue'
import FooterMenu from '@/components/FooterMenuComponent.vue'
export default {
name: 'SiteFooter',
components: {
    GoUp,
    FooterMenu,
}
}
</script>

<style lang="scss" scoped>
footer {
  position: relative;
  background-color: $Dark-bg-color;
    h6 {
      color: $Light-Dark-color;
    }
  }
</style>