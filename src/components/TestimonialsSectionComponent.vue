<template>
  <div class="row_testimonials">
        <div class="row row-cols-1 row-cols-md-2">
          <div class="col py_4 text-center bg_left">
            <div class="text_story">
              <span class="text-uppercase">real stories</span>
              <p class="py-4" v-html="Testimonials[ActiveTestimonial].text"></p>
            </div>
            <!-- /.text_story -->
            <div class="testimonial">
              <img :src="Testimonials[ActiveTestimonial].avatar">
              <h6 class="pt-4 pb-2 mb-0 text-capitalize">{{Testimonials[ActiveTestimonial].name}}</h6>
              <span>{{Testimonials[ActiveTestimonial].work}}</span>
            </div>
            <!-- /.testimonial -->
            <div class="slider_button d-flex flex-column justify-content-center align-items-center">
              <div class="top_arrow" @click="NextTestimonial">
                <img src="@/assets/img/image.png" alt="">
              </div>
              <div class="center_value">
                <span>{{ActiveTestimonial + 1 + '/4'}}</span>
              </div>
              <div class="bottom_arrow" @click="PrecedentTestimonial">
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
name: 'TestimonialsSectionComponent',
data () {
    return {
        ActiveTestimonial: 0,
        Testimonials: [
            {
                avatar: require('@/assets/img/testimonial-avata-02.jpg'),
                text: 'I am free to learn at my own pace, follow<br> my own schedule and choose the subject i<br> want to learn from the syllabus. Great<br> study portal for people like me.',
                name: 'mina hollace',
                work: '/ Freelancer'
            },
            {
                avatar: require('@/assets/img/testimonial-avata-01.jpg'),
                text: ' Lorem ipsum, dolor sit amet consectetur adipisicing elit. Neque, sit ut<br> my own schedule and choose the subject i<br> want to learn from the syllabus. Great<br> study portal for people like me.',
                name: 'mimmo lace',
                work: '/ Manager'
            },
            {
                avatar: require('@/assets/img/testimonial-avata-03.jpg'),
                text: 'I am free to learn at my own pace, follow<br>  Lorem ipsum, dolor sit amet consectetur adipisicing elit. Neque, sit ut<br> want to learn from the syllabus. Great<br> study portal for people like me.',
                name: 'michael red',
                work: '/ Artist'
            },
            {
                avatar: require('@/assets/img/testimonial-avata-04.jpg'),
                text: 'I am free to learn at my own pace, follow<br> my own schedule and choose the subject i<br>  Lorem ipsum, dolor sit amet consectetur adipisicing elit. Neque, sit ut<br> study portal for people like me.',
                name: 'oliver jass',
                work: '/ Author'
            }
        ],
    }
},
methods: {
    NextTestimonial() {
        if (this.ActiveTestimonial == this.Testimonials.length - 1) {
            this.ActiveTestimonial = 0;
        } else {
            this.ActiveTestimonial++;
        }
    },
    PrecedentTestimonial() {
        if (this.ActiveTestimonial == 0) {
            this.ActiveTestimonial = this.Testimonials.length - 1;
        } else {
            this.ActiveTestimonial--;
        }
    }
}
}
</script>

<style lang="scss" scoped>
.row_testimonials {
    padding: 4rem 12px;
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
      max-width: 100%;
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