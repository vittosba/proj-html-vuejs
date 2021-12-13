<template>
    <header>
        <div class="container">
            <!-- nav -->
            <nav>
                <div class="right-nav">
                    <img src="@/assets/avadabarbers-logo-x1.png" alt="">
                </div>
                <div class="left-nav">
                    <i class="fas fa-shopping-cart"></i>
                    <i class="fas fa-bars"></i>
                </div>

            </nav>

            <!-- jumbotron -->
            <div class="jumbotron">
                <div class="row align-items-center">
                    <div class="col-6 left-side">
                        <h1>Barber Shop</h1>
                        <hr>
                        <p>The Pinnacle of Male Grooming</p>
                        <button class="site-btn">Learn More</button>
                    </div>
                    <div class="col-6 right-side">
                        <img src="@/assets/avadabarbers_hero_focalmirror-400x550.png" alt="">
                    </div>
                </div>
            </div>

            <div class="buttons">
                    <img src="@/assets/demos.png" alt="">
                    <img src="@/assets/on-sale.png" alt="">
            </div>
        </div>
    </header>
</template>

<script>
export default {
    name: 'Header',
}
</script>

<style scoped lang="scss">
@import '@/styles/globals';
@import '@/styles/variables';

    header {
        position: relative;
        background-image: url('../assets/avadabarbers-homepage-hero-bg.jpg');
        background-size: cover;
        background-position: center;
        color: $sec-col;
        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding-top: 10px;
    
            .left-nav {
                i {
                    font-size: 1.2rem;
                    margin-left: 10px;
                    cursor: pointer;
                }
            }
        }

        .jumbotron {
            padding-bottom: 70px;

            .row {
                .right-side {
                    display: flex;
                    justify-content: center;
                }

                .left-side {
                    hr {
                        width: 25%;
                        border: 1.5px solid $pri-col;
                        opacity: 1;
                    }
                    p {
                        padding: 1rem 0;
                    }
                }
            }

        }

        .buttons {
            display: flex;
            flex-direction: column;
            position: absolute;
            top: 150px;
            right: 20px;

            img {
                width: 50px;
                margin-bottom: 10px;
                cursor: pointer;
            }
        }
    }
</style>