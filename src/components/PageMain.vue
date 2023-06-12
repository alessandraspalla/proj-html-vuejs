<script>
export default {
    name: 'PageMain'
}
</script>

<template>
    <main>
        <section id="delivery-methods">
            <div class="container">
                <div class="col">
                    <span class="light-color">WHAT WE DO</span>
                    <h2>We offer a full range of
                        <span>
                            <div class="bg"></div>delivery
                        </span> methods.
                    </h2>
                </div>
                <div class="col-60 methods">
                    <div class="icon">
                        <i class="fa-solid fa-truck-fast"></i>
                        <a href="#">
                            <i class="fa-solid fa-arrow-right"></i>
                        </a>
                    </div>
                    <h3>Shipping Fast</h3>
                    <div class="description">
                        Special fast delivery service that guarantees the arrival of the object on the same day as postage.
                        Included monitoring via mobile app.
                    </div>
                </div>
                <div class="col methods">
                    <div class="icon">
                        <i class="fa-solid fa-motorcycle"></i>
                        <a href="#">
                            <i class="fa-solid fa-arrow-right"></i>
                        </a>
                    </div>
                    <h3>Motoboy</h3>
                    <div class="description">
                        Functional motoboy for delivery of documents and small objects.
                    </div>
                </div>
                <div class="col methods">
                    <div class="icon">
                        <i class="fa-solid fa-van-shuttle"></i>
                        <a href="#">
                            <i class="fa-solid fa-arrow-right"></i>
                        </a>
                    </div>
                    <h3>Shuttle Van</h3>
                    <div class="description">
                        Suitable for medium sized loads that need digital tracking.
                    </div>
                </div>
                <div class="col methods">
                    <div class="icon">
                        <i class="fa-solid fa-truck"></i>
                        <a href="#">
                            <i class="fa-solid fa-arrow-right"></i>
                        </a>
                    </div>
                    <h3>Mini Truck</h3>
                    <div class="description">
                        For dry cargo deliveries with more cubic allocation.
                    </div>
                </div>
            </div>
        </section>
    </main>
</template>

<style lang="scss" scoped>
@use './../styles/variables' as *;

#delivery-methods {
    background-color: #111117;
    min-height: 500px;
    padding-block: 80px;

    .container {
        display: flex;
        flex-wrap: wrap;

        .light-color {
            color: $primary-color;
        }

        .icon {
            display: flex;
            justify-content: space-between;

            i {
                color: $primary-color;
                font-size: 2rem;
            }

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
                font-size: 2.8rem;
                line-height: 2.9rem;
                font-weight: 900;

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

        h3 {
            color: $white;
            margin-block: 20px;
        }

        .description {
            color: $white;
            font-weight: 500;
        }
    }

}
</style>