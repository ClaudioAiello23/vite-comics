<!-- PARTE VUE JS-->
<script>
import AppHeaderNav from './AppHeaderNav.vue';
import AppHeaderLogo from './AppHeaderLogo.vue';

export default {
    name: 'AppHeader',
    components: {
        AppHeaderNav,
        AppHeaderLogo
    },

    data() {
        return {

        }
    }
}
</script>

<!-- PARTE HTML -->
<template>
    <header>
        <!-- Collegamento Logo -->
        <AppHeaderLogo />
        <!-- Collegamento menu Nav -->
        <AppHeaderNav />
    </header>
</template>

<!-- PARTE SCSS-->
<style lang="scss" scoped>
header {
    padding: 1.25rem 0;
    display: flex;
    justify-content: space-between;
    align-items: center;
    border-bottom: 1px solid black;
}
</style>