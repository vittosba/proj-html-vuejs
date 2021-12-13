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
                      <div v-for="(service, index) in services" :key="`${index}-service`" class="col-4 px-5 text-center">
                          <img :src='require(`../assets/${service.img}.png`)' alt="">
                          <h3>{{service.title}}</h3>
                          <p>{{service.text}}</p>
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
                      <div v-for="(product, index) in products" :key="`product-${index}`" class="col-3 text-center">
                          <img :src="require(`@/assets/${product.img}.png`)" alt="">
                          <h3>{{product.title}}</h3>
                          <h5>{{product.price}}</h5>
                      </div>
                  </div>
                  <button class="site-btn">Shop our produduct range</button>
              </div>
          </div>

          <!-- reviews -->
          <div class="reviews-section">
              <div class="container">
                <div class="call-to-action">
                    <div class="row justify-content-center">
                        <div class="col-4 text-center">
                            <img src="@/assets/shaving_butter-400x400.png" alt="">
                        </div>
                        <div class="col-6">
                            <h4>This months featured product</h4>
                            <h2>Shaving Butter</h2>
                            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Distinctio, voluptatem suscipit nemo cum quis molestias in, nihil autem maxime accusantium odit rerum alias quibusdam voluptate repudiandae neque? Animi, molestiae natus.</p>
                            <button class="site-btn">Buy now</button>
                        </div>
                    </div>
                </div>
                <div class="reviews text-center">
                    <h4>What people say</h4>
                    <h2>Reviews</h2>
                    <div class="row">
                        <div v-for="(review, index) in reviews" :key="`review-${index}`" class="col-4 px-5 text-center">
                            <p>{{review.text}}</p>
                            <img :src="require(`@/assets/${review.img}.jpg`)" alt="">
                            <h5>{{review.name}}</h5>
                        </div>
                    </div>
                </div>
              </div>
          </div>

          <!-- blog posts -->
          <div class="blog-posts">
              <div class="container">
                  <h4>Tales From The Barber Shop</h4>
                  <h2>Recent Blog Posts</h2>
                  <div class="row">
                      <div v-for="(blogPost, index) in blogPosts" :key="`blogPost-${index}`" class="col-4 px-5 text-center">
                          <img :src="require(`@/assets/${blogPost.img}.jpg`)" alt="">
                          <h3>{{blogPost.title}}</h3>
                          <p>{{blogPost.text}}</p>
                      </div>
                  </div>
                  <button class="site-btn">Read more fro our blog</button>
              </div>
          </div>

  </main>
</template>

<script>
export default {
    name: 'Main',
    data() {
        return {
            services: [
                {
                    img: 'avadabarbers-trimcut-icon-before',
                    title: 'Trim & Cut',
                    text: 'Avada Barbers are expert in the lickety trim and hair cut. Quick but careful amnd ridiculously good looking.'
                },
                {
                    img: 'avadabarbers-washndry-icon',
                    title: 'Wash & Dry',
                    text: 'Taking a seat in our fine leather chairs, lean bacj and let us lather you a fresh head in a luxurious fashion.'
                },
                {
                    img: 'avadabarbers-beardtrim-icon',
                    title: 'Beard Tidy',
                    text: 'Tame the tangles and untidy facial hairs like a gentleman with our Beard Tidy services from Avada Barbers.',
                },
            ],
            products: [
                {
                    img: 'brush_dark-400x400',
                    title: 'Brush',
                    price: '$15.00', 
                },
                {
                    img: 'scissors-400x400',
                    title: 'Scissors',
                    price: '$85.00',
                },
                {
                    img: 'hot_oil_dark-400x400',
                    title: 'Hot Oil',
                    price: '$15.00',
                },
                {
                    img: 'straight_razor_dark-400x400',
                    title: 'Straight Razor',
                    price: '$30.00',
                },
            ],
            reviews: [
                {
                    text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Quod perferendis dignissimos debitis omnis laboriosam pariatur, illum harum dicta corporis aliquam voluptas praesentium dolore velit architecto eveniet minus. Provident, beatae eos!',
                    img: 'avadabarbers-trimcut-gallery6-200x200',
                    name: 'John Doe',
                },
                {
                    text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Quod perferendis dignissimos debitis omnis laboriosam pariatur, illum harum dicta corporis aliquam voluptas praesentium dolore velit architecto eveniet minus. Provident, beatae eos!',
                    img: 'avadabarbers-trimcut-gallery7-200x201',
                    name: 'Pete Jones',
                },
                {
                    text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Quod perferendis dignissimos debitis omnis laboriosam pariatur, illum harum dicta corporis aliquam voluptas praesentium dolore velit architecto eveniet minus. Provident, beatae eos!',
                    img: 'avadabarbers-trimcut-gallery3-200x201',
                    name: 'Mark Wilson',
                },
            ],
            blogPosts: [
                {
                    img: 'avadabarbers-second-blog-700x441',
                    title: 'Avada Barbers Now Open',
                    text: 'Lorem ipsum dolor, sit amet consectetur adipisicing elit. Sint provident fugiat reprehenderit. Ducimus provident eligendi neque officiis corrupti asperiores, non deserunt voluptate, autem alias suscipit commodi, optio sapiente? Quidem, soluta.'
                },
                {
                    img: 'avadabarbers-choosing-blog-700x441',
                    title: 'Choosing The Right Barber',
                    text: 'Lorem ipsum dolor, sit amet consectetur adipisicing elit. Sint provident fugiat reprehenderit. Ducimus provident eligendi neque officiis corrupti asperiores, non deserunt voluptate, autem alias suscipit commodi, optio sapiente? Quidem, soluta.'
                },
                {
                    img: 'avadabarbers-ourservice-blog-700x441',
                    title: 'Quick Service Guide',
                    text: 'Lorem ipsum dolor, sit amet consectetur adipisicing elit. Sint provident fugiat reprehenderit. Ducimus provident eligendi neque officiis corrupti asperiores, non deserunt voluptate, autem alias suscipit commodi, optio sapiente? Quidem, soluta.',
                },
            ],

        }
    }
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

    .reviews-section {
        .container {
            .call-to-action {
                transform: translateY(-20px);
    
                .col-4 {
                    background-image: url('../assets/avadabarbers-cta-background.jpg');
                    background-size: cover;
                    border-top: 2px solid $pri-col;

    
                    img {
                        max-width: 100%;
                    }
                }

                .col-6 {
                    background: #000;
                    padding: 4rem 3rem;
                    border-top: 2px solid $pri-col;
                }
            }

            .reviews {
                padding: 5rem 0;

                img {
                    width: 40%;
                    border-radius: 50%;
                    margin: 10px;
                }
            }
        }

    }

    .blog-posts {
        background: #f5f5f5;
        padding: 5rem 0;

        img {
            max-width: 100%;
        }
    }

</style>