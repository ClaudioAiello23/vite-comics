<!-- PARTE VUE JS-->
<script>
export default {
    name: 'AppMainIconsS',
    data() {
        return {
            icons: [
                {
                    iconImg: 'buy-comics-digital-comics.png',
                    iconName: 'DIGITAL COMICS',
                },
                {
                    iconImg: 'buy-comics-merchandise.png',
                    iconName: 'DC MERCHANDISE',
                },
                {
                    iconImg: 'buy-comics-subscriptions.png',
                    iconName: 'SUBSCRIPTION',
                },
                {
                    iconImg: 'buy-comics-shop-locator.png',
                    iconName: 'COMIC SHOP LOCATOR',
                },
                {
                    iconImg: 'buy-dc-power-visa.svg',
                    iconName: 'DC POWER VISA',
                },
            ]
        }

    }
}
</script>

<!-- PARTE HTML -->
<template>
    <div class="icon_container">
        <div class="icon_box" v-for="icon in icons">
            <div class="img_box">
                <img v-bind:src="'images/' + icon.iconImg" alt="img">
            </div>
            <div class="icon_name"> {{ icon.iconName }}</div>
        </div>
    </div>
</template>

<!-- PARTE SCSS-->
<style lang="scss" scoped>
.icon_container {
    display: flex;
    justify-content: space-between;
}

.icon_box {
    display: flex;
    align-items: center;
    padding: 2.5rem 1.875rem;

    .img_box {
        width: 2.5rem;
        height: 3.125rem;
        margin-right: 0.625rem;

        img {
            width: 100%;
        }
    }

    .icon_name {
        font-size: .8125rem;
    }
}
</style>