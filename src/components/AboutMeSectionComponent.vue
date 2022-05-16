<template>
   <div class="row row_about_me py_4">

        <div class="col-12 col-md-6 col-lg-5">
          <span class="text-uppercase">about me</span>
          <h2 class="title py-3">How to Be an Alpha <br> Male: The 15 Habits of <br> True Alphas</h2>
        </div>
        <!-- /.col -->

        <div class="col-12 col-md-6 col-lg-7 pt-5 d-flex flex-column align-items-end">
          <h5>Want to learn how to be <span class="fs-5">an alpha male</span>? How to be more masculine? <br> How to be the man you've always wanted to be?</h5>
          <p>Your goal is to show the consistency of business, core values, and customer care.<br> Punctuality, responsibility, individuality, accuracy, enthusiasm-you have to clearly<br> explain how these qualities are applicable to your work. And the important things is<br> you do love what you do.</p>
        </div>
        <!-- /.col -->

        <div class="col-12 col-md-6 col-lg-7 py_4">
          <div class="yt_video">
            <img class="banner_video" src="@/assets/img/home-movation-video-poster-670x450.jpg" alt="banner-video">
            <img class="yt_logo" src="@/assets/img/icon-youtube-play.png" alt="youtube-player">
          </div>
          <!-- /.yt_video -->
        </div>
        <!-- /.col -->

        <div class="col-12 col-md-6 col-lg-5 py_4 d-flex flex-column align-items-center justify-content-center">
          <div class="container_items">
            <h4 class="title pb-4">"Every morning you have two<br> choices: continue to sleep with<br> your dreams, or wake up and<br> chase them."</h4>
            <img src="@/assets/img/home-movation-shape-01.png" alt="logo-shape">
            <h5 class="pt-3">Kaixa Stark</h5>
            <span class="text-uppercase">wingman</span>
          </div>
          <!-- /.container_items -->
        </div>
        <!-- /.col -->

      </div>
      <!-- /.row about_me -->
</template>

<script>
export default {
name: 'AboutMeSection',
}
</script>

<style lang="scss" scoped>
 .row_about_me {
    color: $Dark-color;
    span {
      font-size: 0.8rem;
      font-weight: 500;
      color: $Primary-color;
    }
    h2 {
      line-height: 3rem;
    }
    p {
      color: $Light-Dark-color;
      font-size: 1rem;
    }
    h5 {
      line-height: 2rem;
    }
    .yt_video {
      position: relative;
      .banner_video {
        box-shadow: 0 8px 15px -7px black;
        width: 100%;
        object-fit: cover;
        border-radius: 5px;
      }
      .yt_logo {
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        max-width: 20%;
      }
    }
    .container_items{
       h4 {
        line-height: 2.5rem;
      }
      h5 {
        color: $Secondary-color;
      }
      span {
        color: $Light-Dark-color;
      }
    }
   
  }
</style>