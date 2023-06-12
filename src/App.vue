<script>
import PageHeader from './components/PageHeader.vue';
import PageMain from './components/PageMain.vue';
import PageFooter from './components/PageFooter.vue';

export default {
    components: {
        PageHeader,
        PageMain,
        PageFooter
    },
    data() {
        return {
            links: [
                {
                    text: 'HOME',
                    url: '#'
                },
                {
                    text: 'SERVICES',
                    url: '#'
                },
                {
                    text: 'ABOUT',
                    url: '#'
                },
                {
                    text: 'PRICING',
                    url: '#'
                },
                {
                    //text: '<i class="fa-thin fa-user"></i>',
                    url: '#'
                },
                {
                    text: 'GET IN TOUCH',
                    url: '#',
                    btn: true
                }
            ]
        }
    }
}
</script>

<template>
    <PageHeader :details="links" />
    <PageMain />
    <PageFooter />
</template>

<style lang="scss">
@use './styles/variables' as *;
@use './styles/general.scss' as *;
</style>
