<script>
export default {
    name: 'PageMain'
}
</script>

<template>
    <main>
        <!-- section with delivery methods -->
        <section id="delivery-methods">
            <div class="container">
                <!-- column -->
                <div class="col">
                    <span class="summary">WHAT WE DO</span>
                    <h2>We offer a full range of
                        <span>
                            <div class="bg"></div>delivery
                        </span> methods.
                    </h2>
                </div>
                <!-- column -->
                <div class="col-60 methods">
                    <div class="icon">
                        <i class="fa-solid fa-truck-fast"></i>
                        <a href="#">
                            <i class="fa-solid fa-arrow-right"></i>
                        </a>
                    </div>
                    <h3>Shipping Fast</h3>
                    <p class="description">
                        Special fast delivery service that guarantees the arrival of the object on the same day as postage.
                        Included monitoring via mobile app.
                    </p>
                </div>
                <!-- column -->
                <div class="col methods">
                    <div class="icon">
                        <i class="fa-solid fa-motorcycle"></i>
                        <a href="#">
                            <i class="fa-solid fa-arrow-right"></i>
                        </a>
                    </div>
                    <h3>Motoboy</h3>
                    <p class="description">
                        Functional motoboy for delivery of documents and small objects.
                    </p>
                </div>
                <!-- column -->
                <div class="col methods">
                    <div class="icon">
                        <i class="fa-solid fa-van-shuttle"></i>
                        <a href="#">
                            <i class="fa-solid fa-arrow-right"></i>
                        </a>
                    </div>
                    <h3>Shuttle Van</h3>
                    <p class="description">
                        Suitable for medium sized loads that need digital tracking.
                    </p>
                </div>
                <!-- column -->
                <div class="col methods">
                    <div class="icon">
                        <i class="fa-solid fa-truck"></i>
                        <a href="#">
                            <i class="fa-solid fa-arrow-right"></i>
                        </a>
                    </div>
                    <h3>Mini Truck</h3>
                    <p class="description">
                        For dry cargo deliveries with more cubic allocation.
                    </p>
                </div>
            </div>
        </section>
        <!-- section about us -->
        <section id="industry-leader">
            <div class="container">
                <div id="text">
                    <span class="summary">WHO WE ARE</span>
                    <h1>Industry Leaders.</h1>
                    <p>
                        With all of this expertise and capability comes an unrivalled commitment to customer service.
                    </p>
                    <p>
                        We will work hard to understand your needs in order to develop a productive, long-term partnership.
                    </p>
                    <button class="btn primary">
                        READ MORE
                    </button>
                </div>
            </div>
        </section>
        <!-- section with pricing table -->
        <section id="pricing-table">
            <div class="container">
                <span class="summary">MONTHLY PLANS</span>
                <h2>Pricing Table</h2>
                <p>
                    We can help you deliver and execute your future, wherever you compete, using the latest technologies,
                    from
                    strategy development to implemention.
                </p>
                <!-- row with d-flex -->
                <div class="row">
                    <!-- card -->
                    <div class="card">
                        <i class="fa-solid fa-rocket"></i>
                        <h3>Standard</h3>
                        <span>$ <strong>490</strong> / mo</span>
                        <ul>
                            <li>
                                National Coverage
                                <i class="fa-solid fa-check"></i>
                            </li>
                            <li>
                                Unlimited Motoboy
                                <i class="fa-solid fa-check"></i>
                            </li>
                            <li>
                                Address Collection
                                <i class="fa-solid fa-xmark"></i>
                            </li>
                            <li>
                                Mobile App Training
                                <i class="fa-solid fa-xmark"></i>
                            </li>
                            <li>
                                Cargo Insurance
                                <i class="fa-solid fa-xmark"></i>
                            </li>
                        </ul>
                    </div>
                    <!-- card with best price -->
                    <div class="card scale">
                        <div class="label">
                            Most Popular
                        </div>
                        <i class="fa-solid fa-briefcase"></i>
                        <h3>Professional</h3>
                        <span>$ <strong>890</strong> / mo</span>
                        <ul>
                            <li>
                                National Coverage
                                <i class="fa-solid fa-check"></i>
                            </li>
                            <li>
                                Unlimited Motoboy
                                <i class="fa-solid fa-check"></i>
                            </li>
                            <li>
                                Address Collection
                                <i class="fa-solid fa-check"></i>
                            </li>
                            <li>
                                Mobile App Training
                                <i class="fa-solid fa-xmark"></i>
                            </li>
                            <li>
                                Cargo Insurance
                                <i class="fa-solid fa-xmark"></i>
                            </li>
                        </ul>
                    </div>
                    <!-- card -->
                    <div class="card">
                        <i class="fa-solid fa-gem"></i>
                        <h3>Ultimate</h3>
                        <span>$ <strong>1390</strong> / mo</span>
                        <ul>
                            <li>
                                National Coverage
                                <i class="fa-solid fa-check"></i>
                            </li>
                            <li>
                                Unlimited Motoboy
                                <i class="fa-solid fa-check"></i>
                            </li>
                            <li>
                                Address Collection
                                <i class="fa-solid fa-check"></i>
                            </li>
                            <li>
                                Mobile App Training
                                <i class="fa-solid fa-check"></i>
                            </li>
                            <li>
                                Cargo Insurance
                                <i class="fa-solid fa-check"></i>
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
        </section>
        <!-- section with slogan why choose us -->
        <section id="slogan">
            <div class="text">
                <h1>
                    Why choose <span>
                        <span class="bg"></span>us?
                    </span>
                </h1>
                <p>
                    We work intensively in search of ideals that can add up in the lives of our customers. This is what
                    motivates us to improve every day.
                </p>
                <a href="#form" class="btn primary">
                    GET IN TOUCH
                </a>
            </div>
        </section>
    </main>
</template>

<style lang="scss" scoped>
@use './../styles/variables' as *;

i {
    color: $primary-color;
    font-size: 2rem;
}

/* delivery-methods section style */
#delivery-methods {
    background-color: #111117;
    padding-block: 80px;

    .container {
        display: flex;
        flex-wrap: wrap;

        .icon {
            display: flex;
            justify-content: space-between;

            .fa-arrow-right {
                font-size: 1.5rem;
                opacity: .5;
            }
        }

        .col {
            width: calc(100% / 3 - 40px);
            margin: 20px;
            min-height: 200px;
            border-radius: 10px;

            h2 {
                color: $white;

                span {
                    position: relative;
                    z-index: 1;

                    .bg {
                        width: 180px;
                        height: 1.4rem;
                        background-color: $primary-color;
                        border-radius: 5px;
                        position: absolute;
                        left: 0;
                        bottom: 3px;
                        z-index: -1;
                    }
                }
            }
        }

        .col-60 {
            width: calc((100% / 3 - 40px) * 2 + 40px);
            margin: 20px;
            height: 205px;
            border-radius: 10px;
        }

        .methods {
            padding: 30px;
            background-color: #19191f;
        }

        .description,
        h3 {
            color: $white;
        }
    }

}

/* industry-leader section style */
#industry-leader {
    height: 580px;
    background-image: url('/img/bg-6.jpg');
    background-size: cover;
    background-position: 0 -60px;

    .container {
        display: flex;
        justify-content: end;
        align-items: center;
        height: 100%;

        #text {
            width: 40%;

            h1,
            p {
                color: $title-color;
            }

            p {
                margin-block: 20px;
            }
        }

    }


}

/* pricing-table section style */
#pricing-table {
    text-align: center;
    padding-block: 80px;
    background-color: #eef4ed;

    span {
        display: inline-block;
        color: $primary-color;
        margin-bottom: 20px;

        strong {
            font-size: 2rem;
        }
    }

    h2,
    p {
        color: $title-color;
    }

    p {
        width: 60%;
        margin: 20px auto;
    }

    .row {
        display: flex;
        justify-content: space-between;
        margin-top: 50px;

        .card.scale {
            transform: scale(1.09);
            position: relative;
            box-shadow: 3px 7px lightgray;

            .label {
                text-align: left;
                font-size: .65rem;
                color: $white;
                padding: 3px;
                width: 50px;
                height: 30px;
                border-radius: 0 20px 20px 0;
                background-color: #0da6a6;
                position: absolute;
                left: 0;
                top: 20px;
            }
        }

        .card {
            width: 30%;
            background-color: $white;
            padding: 40px 25px;
            border-radius: 10px;

            li {
                display: flex;
                justify-content: space-between;
                color: $title-color;
                margin-block: 12px;
                font-size: .9rem;

                i {
                    font-size: 1.1rem;
                }
            }
        }
    }

}

/* slogan section style */
#slogan {
    height: 550px;
    background-image: url('/img/bg-7.jpg');
    background-position: center;
    background-size: cover;
    display: flex;
    align-items: center;
    justify-content: center;

    a {
        display: inline-block;
        margin-top: 15px;
    }

    .text {
        width: 40%;
        text-align: center;

        h1,
        p {
            color: $white;
        }

        span {
            position: relative;
            z-index: 1;

            .bg {
                width: 105px;
                border-radius: 5px;
                height: 1.75rem;
                background-color: $primary-color;
                position: absolute;
                left: 0;
                bottom: 10px;
                z-index: -1;
            }
        }

    }
}
</style>