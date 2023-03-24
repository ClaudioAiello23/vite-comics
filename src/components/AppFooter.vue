<!-- PARTE VUE JS-->
<script>
import AppFooterNav from './AppFooterNav.vue';
import AppFooterBottom from './AppFooterBottom.vue';
import AppFooterLogo from './AppFooterLogo.vue';

export default {
    name: 'AppFooter',
    components: {
        AppFooterNav,
        AppFooterLogo,
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
        <div class="f_container_1">
            <div class="f_box_1">
                <AppFooterNav />
                <AppFooterLogo />
            </div>
        </div>
        <div class="f_container_2">
            <div class="f_box_2">
                <AppFooterBottom />
            </div>
        </div>
    </footer>
</template>

<!-- PARTE SCSS-->
<style lang="scss" scoped>
footer {
    .f_container_1 {
        background-image: url(/images/footer-bg.jpg);
        background-size: cover;

        .f_box_1 {
            display: flex;
        }
    }

    .f_container_2 {
        background-color: #303030;
        position: relative; //impostata pos.relative + z-index:1 per priorità background che nasconde l'eccedenza del logo grande DC
        z-index: 1;
    }
}
</style>
