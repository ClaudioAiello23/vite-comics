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
        <div class="f_container_1">
            <div class="f_box_1">
                <AppFooterNav />
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
        background-image: url(../assets/footer-bg.jpg);
        background-size: cover;
    }

    .f_container_2 {
        background-color: #303030;
    }
}
</style>
