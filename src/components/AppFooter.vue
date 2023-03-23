<!-- PARTE VUE JS-->
<script>
import AppFooterNav from './AppFooterNav.vue';
import AppFooterBottom from './AppFooterBottom.vue';

export default {
    name: 'AppFooter',
    components: {
        AppFooterNav,
        AppFooterBottom
    },
    data() {
        return {
        }

    }
}
</script>

<!-- PARTE HTML -->
<template>
    <footer>
        <AppFooterNav />
        <AppFooterBottom />
    </footer>
</template>

<!-- PARTE SCSS-->
<style lang="scss" scoped>
footer {
    background-image: url(../assets/footer-bg.jpg);
}
</style>
