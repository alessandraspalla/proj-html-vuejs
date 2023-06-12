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
</template>

<style lang="scss" scoped>
@use './../styles/variables' as *;

#contacts {
    height: 40px;
    background-color: $title-color;
    color: $white;

    .container {
        display: flex;
        justify-content: space-between;
        align-items: center;
        height: 100%;

        .contact {
            display: flex;
        }
    }
}
</style>