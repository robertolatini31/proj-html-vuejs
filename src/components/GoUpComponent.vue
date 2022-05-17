<template>
   <div class="go_up d-flex align-items-center justify-content-center">
      <a href="#">
        <font-awesome-icon icon="fa-solid fa-arrow-up-long" />
      </a>
    </div>
    <!-- /.go_up -->
</template>

<script>
export default {
name: 'GoUpComponent'
}
</script>

<style lang="scss" scoped>
 .go_up {
    position: absolute;
    bottom: 5%;
    right: 1%;
    width: 60px;
    height: 60px;
    border-radius: 50%;
    background-color: $Primary-color;
    a {
      text-decoration: none;
      color: white;
      font-size: 1.5rem;
    }
  }
  @media screen and (max-width:"576px") {
  .go_up {
    width: 50px!important;
    height: 50px!important;
    bottom: 15%!important;
    right: 2%!important;
  }
}
</style>