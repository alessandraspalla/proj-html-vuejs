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
                    <span>WHAT WE DO</span>
                    <h2>We offer a full range of delivery methods.</h2>
                </div>
                <div class="col-60">

                </div>
                <div class="col">

                </div>
                <div class="col">

                </div>
                <div class="col">

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

    .container {
        display: flex;
        flex-wrap: wrap;

        .col {
            width: calc(100% / 3 - 40px);
            margin: 20px;
            min-height: 200px;
            border: 1px solid $white;
            border-radius: 10px;
        }

        .col-60 {
            width: calc((100% / 3 - 40px) * 2 + 40px);
            margin: 20px;
            min-height: 200px;
            border: 1px solid $white;
            border-radius: 10px;
        }
    }

}
</style>