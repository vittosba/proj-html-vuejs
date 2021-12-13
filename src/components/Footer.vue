<template>
  <footer>
        <!-- contacts -->
        <div class="contacts">
            <div class="container">
                <div class="row">
                    <div class="col-4 px-5 text-center">
                        <img src="@/assets/avadabarbers_footer_shop_image-500x390.png" alt="">
                        <button class="site-btn">Shop our range now</button>
                    </div>
                    <div class="col-4 px-5 text-center">
                        <img src="@/assets/avadabarbers-logo-x1.png" alt="">
                        <div class="infos">
                            <div class="info">Avada Barbers</div>
                            <div class="info">123 New York Street</div>
                            <div class="info">New York City</div>
                            <div class="info">info@yourwebsite.com</div>
                            <div class="info">+1 (555) 555-1212</div>
                        </div>
                        <h4>Follow us</h4>
                        <div class="social">
                            <i class="fab fa-facebook-f"></i>
                            <i class="fab fa-twitter"></i>
                            <i class="fab fa-youtube"></i>
                            <i class="fab fa-instagram"></i>
                        </div>

                    </div>
                    <div class="col-4 px-5 text-center">
                        <img src="@/assets/avadabarbers_footer_appointment_image-500x390.png" alt="">
                        <button class="site-btn">Shop our range now</button>
                    </div>
                </div>
            </div>
        </div>

          <!-- copyright -->
        <div class="copyright text-center py-4">
            <p>&#169; Copyright 2012-2020 | Avada theme by ThemeFusion | All Rights Reserved | Powered by Wordpress</p>
        </div>

          
  </footer>
</template>

<script>
export default {
    name: 'Footer',
}
</script>

<style scoped lang="scss">
@import '@/styles/globals';
@import '@/styles/variables';

    .contacts {
        background: #0a0b0c;
        padding: 5rem 0;

        .infos {
            margin-top: 2rem;
            margin-bottom: 2rem;

            .info {
                font-size: 0.9rem;
                color: $four-col;
            }
        }
        .social {
            i {
                font-size: 1.2rem;
                margin: 10px 0;
                cursor: pointer;
            }
        }
        
        img {
            max-width: 100%;
        }
    }

    .copyright {
        background: #0e1011;
        
    }
</style>