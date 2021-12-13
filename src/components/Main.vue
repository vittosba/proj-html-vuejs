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

          <!-- products -->

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

        .container {
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;

            h2 {
                margin-bottom: 2rem;
            }
        }
    }
</style>