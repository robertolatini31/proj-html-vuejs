<template>
  <div id="app">
   
   <Header />


  <main>
    <div class="container">
      <DatesComponent />

      <div class="row row-cols-2 row_about_me py_4">

        <div class="col">
          <span class="text-uppercase">about me</span>
          <h2 class="title py-3">How to Be an Alpha <br> Male: The 15 Habits of <br> True Alphas</h2>
        </div>
        <!-- /.col -->

        <div class="col pt-5 d-flex flex-column align-items-end">
          <h6>Want to learn how to be <span>an alpha male</span>? How to be more masculine? <br> How to be the man you've always wanted to be?</h6>
          <p>Your goal is to show the consistency of business, core values, and customer care.<br> Punctuality,responsibility,individuality,accuracy,enthusiasm-you have to clearly<br> explain how these qualities are applicable to your work. And the important things is<br> you do love what you do.</p>
        </div>
        <!-- /.col -->

        

      </div>
      <!-- /.row about_me -->

      
    </div>
    <!-- /.container -->
  </main>

  </div>
</template>

<script>
import Header from '@/components/SiteHeader.vue'
import DatesComponent from '@/components/DatesSectionComponent.vue'
export default {
  name: 'App',
  components: {
    Header,
    DatesComponent,
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
  .row_about_me {
    span {
      font-size: 0.8rem;
      font-weight: 500;
      color: $Primary-color;
    }
    h2 {
      color: $Dark-color;
      line-height: 3rem;
    }
    p {
      color: $Light-Dark-color;
      font-size: 0.775rem;
    }
    h6 {
      font-size: 1rem;
      line-height: 1.8rem;
    }
  }
}

</style>
