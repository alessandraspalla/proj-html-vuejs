<script>
export default {
    name: 'PageHeader',
    props: {
        details: Array
    }
}
</script>

<template>
    <!-- section with contacts -->
    <div id="contacts">
        <div class="container">
            <div id="opening-time">
                <i class="fa-solid fa-clock"></i>
                Open Hours: Mon - Sat - 9:00 - 18:00
            </div>
            <div class="contact">
                <div class="phone">
                    <i class="fa-solid fa-phone"></i>
                    +1 (305) 1234-5678
                </div>
                <div class="email">
                    <i class="fa-solid fa-envelope"></i>
                    hello@example.com
                </div>
                <div class="social">
                    <a href="https://www.facebook.com/">
                        <i class="fa-brands fa-facebook-f"></i>
                    </a>
                    <a href="https://www.twitter.com/">
                        <i class="fa-brands fa-twitter"></i>
                    </a>
                    <a href="https://www.linkedin.com/">
                        <i class="fa-brands fa-linkedin-in"></i>
                    </a>
                </div>
            </div>
        </div>
    </div>
    <!-- header -->
    <header>
        <div class="container">
            <!-- nav with references to main sections -->
            <nav>
                <div id="logo">
                    <img src="/img/logo.svg" alt="logo nex gen">
                </div>
                <ul>
                    <li v-for="link in details">
                        <a :href="link.url" :class="link.btn ? 'btn primary' : ''">
                            {{ link.text }}
                        </a>
                    </li>
                </ul>
            </nav>
            <!-- hero -->
            <div id="jumbotron">
                <span class="summary">EXPRESS DELIVERY</span>
                <h1>What are we going to deliver <span>
                        <div class="bg"></div>today?
                    </span></h1>
                <button class="btn primary">
                    GET IN TOUCH
                </button>
                <button class="btn reverse">
                    READ MORE
                </button>
            </div>
        </div>
    </header>
</template>

<style lang="scss" scoped>
@use './../styles/variables' as *;

/* contacts style */
#contacts {
    height: 40px;
    background-color: $title-color;
    color: $white;
    font-size: .75rem;

    .container {
        display: flex;
        justify-content: space-between;
        align-items: center;
        height: 100%;

        .contact {
            display: flex;
            gap: 20px;

            a {
                color: $white;
            }

            .social i {
                margin-inline: 12px;
            }
        }
    }
}

/* header style */
header {
    height: 550px;
    background-image: url('/img/bg-13.jpg');
    background-position: 0 -50px;
    background-size: cover;
    position: relative;

    a {
        color: $title-color;
        margin-inline: 13px;
        font-size: .85rem;
    }

    nav {
        height: 60px;
        display: flex;
        justify-content: space-between;
        align-items: center;

        #logo {
            width: 8%;
        }

        ul {
            display: flex;
        }
    }

    /* hero style */
    #jumbotron {
        width: 40%;
        position: absolute;
        top: 50%;
        transform: translate(0, -50%);

        h1 {
            color: $title-color;
        }

        h1 span {
            color: $primary-color;
            position: relative;

            .bg {
                background-color: rgba($primary-color, $alpha: .2);
                width: 200px;
                height: 1.8rem;
                position: absolute;
                left: 0;
                bottom: 3px;
            }
        }
    }
}
</style>