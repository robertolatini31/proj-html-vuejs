<template>
  <div class="row_testimonials py_4">
        <div class="row row-cols-1 row-cols-md-2">
          <div class="col py_4 text-center bg_left">
            <div class="text_story">
              <span class="text-uppercase">real stories</span>
              <p class="py-4">I am free to learn at my own pace, follow<br> my own schedule and choose the subject i<br> want to learn from the syllabus. Great<br> study portal for people like me.</p>
            </div>
            <!-- /.text_story -->
            <div class="testimonial">
              <img src="@/assets/img/testimonial-avata-02.jpg" alt="avatar-testimonial">
              <h6 class="pt-4 pb-2 mb-0">Mina Hollace</h6>
              <span>/ Freelancer</span>
            </div>
            <!-- /.testimonial -->
            <div class="slider_button d-flex flex-column justify-content-center align-items-center">
              <div class="top_arrow">
                <img src="@/assets/img/image.png" alt="">
              </div>
              <div class="center_value">
                <span>1/4</span>
              </div>
              <div class="bottom_arrow">
                <img src="@/assets/img/image(1).png" alt="">
              </div>
            </div>
            <!-- /.slider_button -->
          </div>
          <!-- /.col -->
          <div class="col bg_right">
          </div>
          <!-- /.col -->
        </div>
        <!-- /.row -->
      </div>
      <!-- /.row_testimonials -->
</template>

<script>
export default {
name: 'TestimonialsSectionComponent'
}
</script>

<style lang="scss" scoped>
.row_testimonials {
    .bg_left {
      background-image: url('@/assets/img/background-pattern-wavify.png');
      position: relative;
    }
    .text_story {
      span {
        color: $Primary-color;
        font-size: 0.8rem;
        font-weight: 500;
      }
      p {
        line-height: 2rem;
      }
    }
    .testimonial {
      img {
        height: 50px;
        width: 50px;
        border-radius: 50%;
      }
      span {
        font-size: 0.7rem;
        color: $Light-Dark-color;
      }
    }
    .bg_right {
      background-image: url('@/assets/img/home-movation-testimonial-image.jpg');
      background-size: cover;
      background-repeat: no-repeat;
      min-height: 400px;
    }
    .slider_button {
      cursor: pointer;
      position: absolute;
      bottom: calc(50% - 65px);
      right: -65px;
      transform: translate(-50%, -50%);
      height: 65px;
      width: 65px;
      border-radius: 50%;
      background-color: white;
      box-shadow: 0 0 20px -8px black;
      span {
        font-size: 0.8rem;
      }
    }
  }
  @media screen and (max-width:"768px") {
    .slider_button {
      bottom: -65px!important;
      right: calc(50% - 65px)!important;
      transform: translate(-50%, -50%);
    }
    .row_testimonials {
      padding-top: 0!important;
    }
  }
</style>