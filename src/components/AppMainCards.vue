<!-- PARTE VUE JS-->
<script>
export default {
    name: 'AppMainCards',
    data() {
        return {
            cards: [
                {
                    cardImg: 'buy-comics-digital-comics.png',
                    cardName: 'DIGITAL COMICS',
                },
                {
                    cardImg: 'buy-comics-merchandise.png',
                    cardName: 'DC MERCHANDISE',
                },
                {
                    cardImg: 'buy-comics-subscriptions.png',
                    cardName: 'SUBSCRIPTION',
                },
                {
                    cardImg: 'buy-comics-shop-locator.png',
                    cardName: 'COMIC SHOP LOCATOR',
                },
                {
                    cardImg: 'buy-dc-power-visa.png',
                    cardName: 'DC POWER VISA',
                },
            ]
        }

    }
}
</script>

<!-- PARTE HTML -->
<template>
    <div class="card_container">
        <div class="card_box" v-for="(cardTitle, cardImg) in cards">
            <div>
                <img v-bind:src="cardImg.Img" alt="img">
            </div>
            <div class="single_card"> {{ cardTitle.cardName }}</div>
        </div>
    </div>
</template>

<!-- PARTE SCSS-->
<style lang="scss" scoped>
.card_container {
    display: flex;
    justify-content: space-between;
}

.card_box {
    display: flex;
    padding: 3.75rem 1.875rem;
}
</style>