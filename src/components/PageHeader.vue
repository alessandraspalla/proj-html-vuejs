<script>
export default {
    name: 'PageHeader'
}
</script>

<template>
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
                    <i class="fa-brands fa-facebook-f"></i>
                    <i class="fa-brands fa-twitter"></i>
                    <i class="fa-brands fa-linkedin-in"></i>
                </div>
            </div>
        </div>
    </div>
    <header>
        <div class="container">
            <nav>
                <div id="logo">
                    <img src="/img/logo.svg" alt="logo nex gen">
                </div>
                <ul>
                    <li>HOME</li>
                    <li>SERVICES</li>
                    <li>ABOUT</li>
                    <li>PRICING</li>
                    <li>OMINO</li>
                    <li>GET IN TOUCH</li>
                </ul>
            </nav>
            <div id="jumbotron">
                <span>EXPRESS DELIVERY</span>
                <h1>What are we going to deliver today?</h1>
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
            gap: 8px;

            .social i {
                margin-inline: 8px;
            }
        }
    }
}

header {
    min-height: 550px;
    background-image: url('/img/bg-13.jpg');
    background-position: 0 -50px;
    background-size: cover;
    position: relative;

    .btn {
        padding: 10px;
        border-radius: 3px;
        font-size: .8rem;
        margin: 8px;
    }

    .btn.primary {
        color: #fff;
        background-color: $primary-color;
    }

    .btn.reverse {
        color: $primary-color;
        background-color: #fff;
        border: 1px solid $primary-color;
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

    #jumbotron {
        width: 40%;
        position: absolute;
        top: 50%;
        transform: translate(0, -50%);

        span {
            color: #0da6a6;
        }
    }
}
</style>