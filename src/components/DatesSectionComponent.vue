<template>
  <div class="row row-cols-1 row-cols-md-2 row-cols-lg-4 row_dates py_4">
        <div class="col d-flex justify-content-center">
            <img class="left_border left_border_col_1" src="@/assets/img/background-pattern-grid-line-06.png" alt="border-image">
            <div class="text_dates text-center align-self-center">
              <h3 class="mb-3">1.926</h3>
              <span class="text-uppercase">finished sessions</span>
            </div>
            <img class="right_border right_border_col_1" src="@/assets/img/background-pattern-grid-line-06.png" alt="border-image">
        </div>
        <!-- /.col -->
         <div class="col d-flex justify-content-center">
            <img class="left_border left_border_col_2" src="@/assets/img/background-pattern-grid-line-06.png" alt="border-image">
            <div class="text_dates text-center align-self-center">
              <h3 class="mb-3">100%</h3>
              <span class="text-uppercase">satisfaction rate</span>
            </div>
            <img class="right_border right_border_col_2" src="@/assets/img/background-pattern-grid-line-06.png" alt="border-image">
        </div>
        <!-- /.col -->
         <div class="col d-flex justify-content-center">
            <img class="left_border left_border_col_3" src="@/assets/img/background-pattern-grid-line-06.png" alt="border-image">
            <div class="text_dates text-center align-self-center">
              <h3 class="mb-3">3092+</h3>
              <span class="text-uppercase">enrolled learners</span>
            </div>
            <img class="right_border right_border_col_3" src="@/assets/img/background-pattern-grid-line-06.png" alt="border-image">
        </div>
        <!-- /.col -->
         <div class="col d-flex justify-content-center">
            <img class="left_border left_border_col_4" src="@/assets/img/background-pattern-grid-line-06.png" alt="border-image">
            <div class="text_dates text-center align-self-center">
              <h3 class="mb-3">200</h3>
              <span class="text-uppercase">online instructors</span>
            </div>
            <img class="right_border right_border_col_4" src="@/assets/img/background-pattern-grid-line-06.png" alt="border-image">
        </div>
        <!-- /.col -->
      </div>
      <!-- /.row row_dates -->
</template>

<script>
export default {
name: 'DatesSectionComponent',
}
</script>

<style lang="scss" scoped>
.row_dates {
    .col {
      position: relative;
      height: 100px;

      img {
        position: absolute;
        height: 100px;

      }
      .left_border {
        top: 0;
        left: 0;
      }
      .right_border {
        top: 0;
        right: 0;
        transform: rotate(180deg);
      }
      h3 {
        color: $Primary-color;
      }
      span {
        font-size: 0.9rem;
        font-weight: 500;
      }
    }
  }
@media screen and (min-width:"768px") {
  .right_border_col_1 {
    display: none;
  }
  .right_border_col_3 {
    display: none;
  }
}
@media screen and (min-width:"992px") {
  .right_border_col_2 {
    display: none;
  }
}
</style>