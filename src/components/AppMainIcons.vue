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
                    iconImg: 'buy-dc-power-visa.png',
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
        <div class="icon_box" v-for="(iconTitle, iconImg) in icons">
            <div>
                <img v-bind:src="iconImg.iconImg" alt="img">
            </div>
            <div class="single_card"> {{ iconTitle.iconName }}</div>
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
    padding: 3.75rem 1.875rem;
}
</style>