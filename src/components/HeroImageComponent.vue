<template>
  <div class="hero_image pt-5">
        <div class="row row-cols-1 row-cols-lg-2 hero_row">
          <div class="col col_hero_text d-flex pt-4">
             <div class="hero_text align-self-center">
                <span class="text-uppercase">i'm wingman</span>
              <h1 class="title pb-4 m-0 pt-4 text-capitalize">peace on earth a <br> wonderful wish <br> but no way</h1>
              <p class="m-0 pb-4">Success isn't overnight. It's when everyday you get a little <br> better than day before. it all adds up.</p>
              <button class="mb-5">
                <div class="button_text d-flex">
                  <span class="text-capitalize me-2">get started for free</span>
                  <font-awesome-icon class="align-self-center" icon="fa-solid fa-arrow-right-long" />
                </div>
              </button>
             </div>
             <!-- /.hero_text -->
          </div>
          <!-- /.col -->
          <div class="col col_hero_img" @mousemove="MouseMoved"  :style="{ 'background-position' : `${x}px ${y}px` }">
            <img class="big_img_hero big_hero_image" src="@/assets/img/home-movation-hero-image.png" alt="hero_image">
            <img class="big_img_hero small_hero_image" src="@/assets/img/home-movation-hero-image-246x300.png" alt="hero_image">
          </div>
          <!-- /.col -->
        </div>
        <!-- /.row -->
      </div>
      <!-- /.hero_image -->
</template>

<script>
export default {
name: 'HeroImageComponent',
data () {
  return {
    x: 70,
    y: 100,
  }
},
methods: {
  MouseMoved(e) {
    this.x = 70 - e.offsetX / 20 ;
    this.y = 100 - (e.offsetY / 20);
  }
}
}
</script>

<style lang="scss" scoped>
  .hero_image {
  .hero_text {
    color: $Dark-color;
    h1 {
      line-height: 3.5rem;
    }
    span, p, .button_text {
      font-size: 0.8rem;
    }
    span {
    font-weight: 500;
    }
    p {
      color: $Light-Dark-color;
    }
    button {
      border: none;
      border-radius: 5px;
      background-color: $Primary-color;
      .button_text {
        font-weight: 500;
        color: white;
        padding: 0.8rem 2.5rem;
      }
    }
    button:hover {
      background-color: $Secondary-color;
    }
  }

  .col_hero_img {
    background-image: url('@/assets/img/home-movation-shape-face.png');
    background-repeat: no-repeat;
    background-position: bottom;
    background-size: 450px;
    img {
      max-height: 500px;
    }
    .small_hero_image {
      display: none;
    }
  }
}
@media screen and (max-width:"992px") {
  .hero_row {
    flex-direction: column;
    .col_hero_text {
        justify-content: center!important;
        .hero_text {
            text-align: center;
        }
    }
   
  }
}
@media screen and (max-width:"576px") {
  .big_hero_image {
    display: none;
  }
  .small_hero_image {
    display: inline!important;
  }
}
</style>