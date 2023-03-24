<!-- PARTE VUE JS-->

<script>
export default {
    name: 'AppFooterBottom',
    data() {
        return {
            socials: [
                {
                    socialImg: 'footer-facebook.png',
                    socialName: 'FACEBOOK',
                },
                {
                    socialImg: 'footer-twitter.png',
                    socialName: 'TWITTER',
                },
                {
                    socialImg: 'footer-youtube.png',
                    socialName: 'YOUTUBE',
                },
                {
                    socialImg: 'footer-pinterest.png',
                    socialName: 'PINTEREST',
                },
                {
                    socialImg: 'footer-periscope.png',
                    socialName: 'PERISCOPE',
                }
            ]
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
            <div class="social_icons" v-for="social in socials">
                <a href="#"><img v-bind:src="'images/' + social.socialImg" alt="img"></a>
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
    align-items: center;

    button {
        background-color: #303030;
        color: white;
        padding: .9375rem;
        border: 2px solid $text-second-color;
        cursor: pointer;
    }

    .social {
        display: flex;
        align-items: center;

        .follow {
            color: $text-second-color;
            font-weight: bold;
            padding-right: 1.25rem;
        }

        .social_icons {
            padding-left: .9375rem;
        }
    }
}
</style>