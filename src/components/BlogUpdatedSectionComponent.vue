<template>
  <div class="row_blog_update py_4">
        <div class="titles">
          <span class="text-uppercase">blog update</span>
          <h2 class="title py-3">Intereesting <span class="fs-2">articles update</span> daily</h2>
        </div>
        <!-- /.titles -->
        <div class="row row-cols-1 row-cols-md-2 row-cols-lg-4 py-3">
            <div class="col mb-4">
              <div class="article_card">
                <img src="@/assets/img/motivation-blog-04-480x325.jpg">
                <div class="text_card py-3">
                  <span>
                    <font-awesome-icon class="me-2" icon="fa-regular fa-calendar" />
                    May 13, 2020
                  </span>
                  <h6 class="py-2">How to Stay True to Your Personal Brand</h6>
                  <span>When it comes to your business or career, you want ...</span>
                </div>
                <!-- /.text_card -->
              </div>
              <!-- /.article_card -->
            </div>
            <!-- /.col -->
             <div class="col mb-4">
              <div class="article_card">
                <img src="@/assets/img/motivation-blog-03-480x325.jpg">
                <div class="text_card py-3">
                  <span>
                    <font-awesome-icon class="me-2" icon="fa-regular fa-calendar" />
                    May 13, 2020
                  </span>
                  <h6 class="py-2">5 Vital Lessons in 5 Years of Freelancing</h6>
                  <span>Being self-employed and working from home, it's easy to get ...</span>
                </div>
                <!-- /.text_card -->
              </div>
              <!-- /.article_card -->
            </div>
            <!-- /.col -->
            <div class="col mb-4">
              <div class="article_card">
                <img src="@/assets/img/motivation-blog-02-480x325.jpg">
                <div class="text_card py-3">
                  <span>
                    <font-awesome-icon class="me-2" icon="fa-regular fa-calendar" />
                    May 13, 2020
                  </span>
                  <h6 class="py-2">11 Super Useful Tips for Small-Business Owners</h6>
                  <span>Being a small-business owner poses a ton of challenges. We ...</span>
                </div>
                <!-- /.text_card -->
              </div>
              <!-- /.article_card -->
            </div>
            <!-- /.col -->
            <div class="col mb-4">
              <div class="article_card">
                <img src="@/assets/img/motivation-blog-01-480x325.jpg">
                <div class="text_card py-3">
                  <span>
                    <font-awesome-icon class="me-2" icon="fa-regular fa-calendar" />
                    May 13, 2020
                  </span>
                  <h6 class="py-2">How to Give Yourself Grace to Start Again</h6>
                  <span>Forgive yourself for bad habits you may have started or ...</span>
                </div>
                <!-- /.text_card -->
              </div>
              <!-- /.article_card -->
            </div>
            <!-- /.col -->
        </div>
        <!-- /.row -->
        <div class="all_posts text-center">
          <a href="#" class="text-uppercase pb-1">view all posts</a>
        </div>
        <!-- /.all_posts -->
      </div>
      <!-- /.row_blog_update -->
</template>

<script>
export default {
name: 'BlogUpdatedSectionComponent',
}
</script>

<style lang="scss" scoped>
.row_blog_update {
    .titles {
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
    }
    .article_card {
      img {
        border-radius: 5px;
      }
      span {
        font-size: 0.8rem;
        color: $Light-Dark-color;
      }
      h6 {
        line-height: 1.8rem;
      }
    }
    .all_posts {
      a {
        color: $Primary-color;
        text-decoration: none;
        border-bottom: 1px solid $Primary-color;
        font-size: 0.8rem;
        font-weight: 500;
      }
    }
  }
</style>