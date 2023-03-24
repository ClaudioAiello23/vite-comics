<!-- PARTE VUE JS-->

<script>
export default {
    name: 'AppHeaderJumbo',
    data() {
        return {

        }
    }
}
</script>

<!-- PARTE HTML -->
<template>
    <div id="h_jumbo_box">
        <img src="/images/jumbotron.jpg" alt="logo">
    </div>
</template>

<!-- PARTE SCSS-->
<style lang="scss" scoped>
#h_jumbo_box {

    img {
        width: 100%;
        height: 400px;
        object-fit: cover; //evita di 'schiacciare' una foto cui viene data un'altezza precisa
        object-position: 10% 1%; //scelgo quale parte far vedere della foto croppata
        display: block; //risolve il problema (da browser) dei 4px bianchi sotto l'img
    }
}
</style>