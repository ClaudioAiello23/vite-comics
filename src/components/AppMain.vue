<!-- PARTE VUE JS-->
<script>
import AppMainPhotos from './AppMainPhotos.vue';
import AppMainCards from './AppMainCards.vue';


export default {
    name: 'AppMain',
    components: {
        AppMainPhotos,
        AppMainCards
    },
    data() {
        return {
        }

    }
}
</script>

<!-- PARTE HTML -->
<template>
    <main>
        <AppMainPhotos />
        <AppMainCards />
    </main>
</template>

<!-- PARTE SCSS-->
<style lang="scss" scoped>
main {
    color: white;
}
</style>