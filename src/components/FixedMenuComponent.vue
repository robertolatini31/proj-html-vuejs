<template>
  <div class="fixed_menu d-flex flex-column">
     <font-awesome-icon class="fixed_icon" icon="fa-solid fa-ruler-combined" />
     <font-awesome-icon class="fixed_icon" icon="fa-solid fa-life-ring" />
     <font-awesome-icon class="fixed_icon" icon="fa-solid fa-book" />
     <font-awesome-icon class="fixed_icon" icon="fa-solid fa-cart-shopping" />
   </div>
   <!-- /.fixed_menu -->
</template>

<script>
export default {
name: 'FixedMenuComponent',
}
</script>

<style lang="scss" scoped>
.fixed_menu {
  z-index: 10000;
  position: fixed;
  top: 130px;
  right: -5px;
  border-radius: 5px;
  background-color: white;
  box-shadow: 0 0 8px -4px black;
  .fixed_icon:hover {
    color: $Primary-color;
  }
  .fixed_icon {
      transition: all .2s;
    padding: 0.8rem;
    font-size: 1rem;
    cursor: pointer;
  }
}

</style>