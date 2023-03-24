<!-- PARTE VUE JS-->

<script>
export default {
    name: 'AppFooterBottom',
    data() {
        return {

        }
    }
}
</script>

<!-- PARTE HTML -->
<template>
    <div class="f_box_2">
        <div><button type="button">SIGN-UP NOW!</button></div>
        <div class="social">
            <div class="follow">FOLLOW US</div>
            <div>
                <ul>
                    <li><a href="#">CBEFG</a></li>
                </ul>
            </div>
        </div>
    </div>
</template>

<!-- PARTE SCSS-->
<style lang="scss" scoped>
@use '../assets/styles/partials/variables' as *;

.f_box_2 {
    padding: 1.875rem 0;
    display: flex;
    justify-content: space-between;

    button {
        background-color: #303030;
        color: white;
        padding: .9375rem;
        border: 2px solid $text-second-color;
        cursor: pointer;
    }

    .social {
        .follow {
            color: $text-second-color;
            font-weight: bold;
        }
    }
}
</style>