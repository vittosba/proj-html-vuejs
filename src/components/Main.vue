<template>
  <main>
          <!-- hero -->
          <div class="hero">
            <div class="container">
              <h4>Award winning</h4>
              <h2>Pro Barbers</h2>
              <button class="site-btn">Meet your new barber</button>
            </div>
          </div>

          <!-- services -->
          <div class="services">
              <div class="container">
                  <h4>Mens Grooming</h4>
                  <h2>Services</h2>
                  <div class="row">
                      <div class="col-4 px-5 text-center">
                          <img src="@/assets/avadabarbers-trimcut-icon-before.png" alt="">
                          <h3>Trim & Cut</h3>
                          <p>Avada Barbers are expert in the lickety trim and hair cut. Quick but careful amnd ridiculously good looking.</p>
                      </div>
                      <div class="col-4 px-5 text-center">
                          <img src="@/assets/avadabarbers-washndry-icon.png" alt="">
                          <h3>Wash & Dry</h3>
                          <p>Taking a seat in our fine leather chairs, lean bacj and let us lather you a fresh head in a luxurious fashion.</p>
                      </div>
                      <div class="col-4 px-5 text-center">
                          <img src="@/assets/avadabarbers-beardtrim-icon.png" alt="">
                          <h3>Beard Tidy</h3>
                          <p>Tame the tangles and untidy facial hairs like a gentleman with our Beard Tidy services from Avada Barbers.</p>
                      </div>
                  </div>
                  <button class="site-btn">Read about our services</button>
              </div>
          </div>

          <!-- products -->
          <div class="products">
              <div class="container">
                  <h4>We have you covered</h4>
                  <h2>Avada Grooming Products</h2>
                  <div class="row">
                      <div class="col-3 text-center">
                          <img src="@/assets/brush_dark-400x400.png" alt="">
                          <h3>Brush</h3>
                          <h4>$15.00</h4>
                      </div>
                      <div class="col-3 text-center">
                          <img src="@/assets/scissors-400x400.png" alt="">
                          <h3>Scissors</h3>
                          <h4>$85.00</h4>
                      </div>
                      <div class="col-3 text-center">
                          <img src="@/assets/hot_oil_dark-400x400.png" alt="">
                          <h3>Hot Oil</h3>
                          <h4>$15.00</h4>
                      </div>
                      <div class="col-3 text-center">
                          <img src="@/assets/straight_razor_dark-400x400.png" alt="">
                          <h3>Straight Razor</h3>
                          <h4>$30.00</h4>
                      </div>
                  </div>
                  <button class="site-btn">Shop our produduct range</button>
              </div>
          </div>

          <!-- reviews -->

          <!-- blog posts -->

  </main>
</template>

<script>
export default {
    name: 'Main',
}
</script>

<style scoped lang="scss">
@import '@/styles/globals';
@import '@/styles/variables';

    .hero {
        background-image: url('../assets/avadabarbers-about-introbackground.jpg');
        padding: 5rem 0;
    }
    .container {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;

        h2 {
            margin-bottom: 2rem;
        }

        h3 {
            margin: 1.5rem 0;
        }
    }

    .services {
        padding: 5rem 0;

        .row {
            padding: 3rem;

            img {
                height: 150px;
            }
        }
    }

    .products {
        background-image: url('../assets/avadabarbers-reviewsbackground.jpg');
        background-position: center;
        background-size: contain;
        padding: 5rem 0;

        .row {
            margin: 2rem 0;

            img {
                max-width: 100%;
            }
        }
    }

</style>