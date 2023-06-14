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
                    url: '#contacts'
                },
                {
                    text: 'SERVICES',
                    url: '#delivery-methods'
                },
                {
                    text: 'ABOUT',
                    url: '#industry-leader'
                },
                {
                    text: 'PRICING',
                    url: '#pricing-table'
                }
            ],
            contacts: [
                {
                    icon: 'fa-solid fa-phone',
                    text: '+1 (305) 1234-5678',
                    type: 'number'
                },
                {
                    icon: 'fa-solid fa-envelope',
                    text: 'hello@example.com',
                    type: 'mail'
                },
                {
                    icon: 'fa-solid fa-location-dot',
                    text: 'Main Avenue, 987',
                    type: 'maps'
                }
            ]
        }
    }
}
</script>

<template>
    <PageHeader :details="links" :contacts="contacts" />
    <PageMain />
    <PageFooter :contacts="contacts" />
</template>

<style lang="scss">
@use './styles/variables' as *;
@use './styles/general.scss' as *;
</style>
