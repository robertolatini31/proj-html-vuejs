<template>
  <div class="row_books pt-4">
        <div class="row book_store pb-4">
          <div class="col-12 col-lg-4 titles_col">
            <span class="text-uppercase">book store online</span>
            <h2 class="title py-3">Be Aplpha With <br> <span class="fs-2">Wingman's Books</span></h2>
              <ul class="p-0 m-0 pb-4 mb-3">
            <li>
              <font-awesome-icon class="icon_check me-2" icon="fa-solid fa-check" />
              <span>Help you understand yourself better</span>
            </li>
            <li>
              <font-awesome-icon class="icon_check me-2" icon="fa-solid fa-check" />
              <span>Revealing mature tips</span>
            </li>
            <li>
              <font-awesome-icon class="icon_check me-2" icon="fa-solid fa-check" />
              <span>Give the right advice</span>
            </li>
            <li>
              <font-awesome-icon class="icon_check me-2" icon="fa-solid fa-check" />
              <span>Fascinating examples of alpha man</span>
            </li>
          </ul>
          <button class="mb-5">
            <div class="button_text d-flex">
              <span class="text-capitalize">get free ebook</span>
            </div>
          </button>
          </div>
          <!-- /.col-4 -->
          <div class="col-12 col-lg-8">
            <div class="row row-cols-1 row-cols-md-2">
              <div class="col">
                <div class="book_card text-center">
                  <img src="@/assets/img/product-book-11-400x400.jpg" alt="book-1">
                  <div class="card_text text-center">
                    <h5 class="py-3">Alpha man by Maxcoach</h5>
                    <span>$29.<small>00</small></span>
                  </div>
                  <!-- /.card_text -->
                  <div class="icons_hover d-flex flex-column">
                    <div class="icon_hover mb-3 d-flex align-items-center justify-content-center">
                      <font-awesome-icon icon="fa-solid fa-magnifying-glass" />
                    </div>
                    <!-- /.icon_hover -->
                    <div class="icon_hover mb-3 d-flex align-items-center justify-content-center">
                      <font-awesome-icon icon="fa-solid fa-cart-shopping" />
                    </div>
                    <!-- /.icon_hover -->
                    <div class="icon_hover mb-3 d-flex align-items-center justify-content-center">
                      <font-awesome-icon icon="fa-regular fa-heart" />
                    </div>
                    <!-- /.icon_hover -->
                    <div class="icon_hover mb-3 d-flex align-items-center justify-content-center">
                      <font-awesome-icon icon="fa-solid fa-signal" />
                    </div>
                    <!-- /.icon_hover -->
                  </div>
                  <!-- /.icons_hover -->
                </div>
                <!-- /.book_card -->
              </div>
              <!-- /.col -->
              <div class="col">
                <div class="book_card text-center">
                  <img src="@/assets/img/product-book-10-400x400.jpg" alt="book-1">
                  <div class="card_text text-center">
                    <h5 class="py-3">Real man 4.0 by Maxcoach</h5>
                    <span>$39.<small>00</small></span>
                  </div>
                  <!-- /.card_text -->
                  <div class="icons_hover d-flex flex-column">
                    <div class="icon_hover mb-3 d-flex align-items-center justify-content-center">
                      <font-awesome-icon icon="fa-solid fa-magnifying-glass" />
                    </div>
                    <!-- /.icon_hover -->
                    <div class="icon_hover mb-3 d-flex align-items-center justify-content-center">
                      <font-awesome-icon icon="fa-solid fa-cart-shopping" />
                    </div>
                    <!-- /.icon_hover -->
                    <div class="icon_hover mb-3 d-flex align-items-center justify-content-center">
                      <font-awesome-icon icon="fa-regular fa-heart" />
                    </div>
                    <!-- /.icon_hover -->
                    <div class="icon_hover mb-3 d-flex align-items-center justify-content-center">
                      <font-awesome-icon icon="fa-solid fa-signal" />
                    </div>
                    <!-- /.icon_hover -->
                  </div>
                  <!-- /.icons_hover -->
                </div>
                <!-- /.book_card -->
              </div>
              <!-- /.col -->
            </div>
            <!-- /.row -->
          </div>
          <!-- /.col-8 -->
        </div>
        <!-- /.row book_store-->
        <div class="row row-cols-2 row-cols-md-3 row-cols-lg-6 logos py_4 align-items-center">
          <div class="col">
            <img src="@/assets/img/client-logo-05-primary.png" alt="its-alive-logo">
          </div>
          <!-- /.col -->
          <div class="col">
            <img src="@/assets/img/client-logo-06-primary.png" alt="its-alive-logo">
          </div>
          <!-- /.col -->
          <div class="col">
            <img src="@/assets/img/client-logo-07-primary.png" alt="its-alive-logo">
          </div>
          <!-- /.col -->
          <div class="col">
            <img src="@/assets/img/client-logo-04-primary.png" alt="its-alive-logo">
          </div>
          <!-- /.col -->
          <div class="col">
            <img src="@/assets/img/client-logo-03-primary.png" alt="its-alive-logo">
          </div>
          <!-- /.col -->
          <div class="col">
            <img src="@/assets/img/client-logo-02-primary.png" alt="its-alive-logo">
          </div>
          <!-- /.col -->
        </div>
        <!-- /.row logos -->
      </div>
      <!-- /.row_books -->
</template>

<script>
export default {
name: 'BookSectionComponent',
}
</script>

<style lang="scss">
.row_books {
    .titles_col {
   span {
     font-size: 0.8rem;
   }
   h2 {
     line-height: 3.5rem;
     color: $Secondary-color;
     span {
       color: $Primary-color;
     }
   }
   ul {
   list-style: none;
   li {
     padding: 0.6rem 0;
     .icon_check {
       color: $Primary-color;
       font-size: 1rem;
     }
     span {
       font-size: 0.8rem;
       color: $Light-Dark-color;
     }
   }
 }
 button {
      border: none;
      border-radius: 5px;
      background-color: $Primary-color;
      .button_text {
        color: white;
        font-weight: 500;
        padding: 0.8rem 2.5rem;
      }
    }
 }
 .book_card:hover .icons_hover{
   display: flex!important;
 }
 .book_card {
   position: relative;
   h5 {
     color: $Secondary-color;
   }
   span {
     color: $Primary-color;
     font-weight: 500;
     font-size: 1.2rem;
   }
   .icons_hover {
     display: none!important;
     position: absolute;
     top: 5%;
     right: 5%;
     .icon_hover {
       box-shadow: 0 0 20px -8px black;
       cursor: pointer;
       height: 50px;
       width: 50px;
       border-radius: 50%;
       background-color: white;
     }
   } 
 }
 .logos {
   .col {
     display: flex;
     justify-content: center;
     margin-bottom: 3rem;
   }
   img {
     filter: grayscale(1) opacity(0.38);
   }
 }
 
}
 @media screen and (max-width:"768px") {
   .icons_hover {
     top: 8%!important;
     right: 16%!important;
   }
 }
 @media screen and (max-width:"480px") {
   .icons_hover {
     top: 8%!important;
     right: 8%!important;
   }
 }
</style>