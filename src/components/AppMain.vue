<!-- PARTE VUE JS-->
<script>
import AppMainCards from './AppMainCards.vue';
import AppMainIcons from './AppMainIcons.vue';


export default {
    name: 'AppMain',
    components: {
        AppMainCards,
        AppMainIcons
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
        <div class="m_container_1">
            <div class="m_box_1">
                <AppMainCards />
            </div>
        </div>
        <div class="m_container_2">
            <div class="m_box_2">
                <AppMainIcons />
            </div>
        </div>
    </main>
</template>

<!-- PARTE SCSS-->
<style lang="scss" scoped>
@use '../assets/styles/partials/variables' as *; //imposto l'uso della variabile dichiarata in assets-styles-partials-variables

main {
    color: $text_first_color; //utilizzo della variabile impostata all'inizio di style

    .m_container_1 {
        background-color: #1c1c1c;
    }

    .m_container_2 {
        background-color: $text_second_color; //utilizzo della variabile impostata all'inizio di style
        position: relative; //impostata pos.relative + z-index:1 per priorità background che nasconde l'eccedenza del logo grande DC
        z-index: 1;
    }
}
</style>