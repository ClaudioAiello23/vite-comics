<!-- PARTE VUE JS-->

<script>
import ItemCardsModel from './ItemCardsModel.vue';

export default {
    name: 'AppMainCards',
    components: {
        ItemCardsModel
    },
    data() {
        return {
            cards: [
                {
                    "thumb": 'https://i.ibb.co/GCN80gY/superman.png',
                    "price": "$19.99",
                    "series": "Action Comics",
                    "type": "comic book"
                },
                {
                    "thumb": "https://i.ibb.co/GCN80gY/superman.png",
                    "price": "$3.99",
                    "series": "American Vampire 1976",
                    "type": "comic book"
                },
                {
                    "thumb": "https://i.ibb.co/GCN80gY/superman.png",
                    "price": "$16.99",
                    "series": "Aquaman",
                    "type": "graphic novel"
                },
                {
                    "thumb": "https://i.ibb.co/GCN80gY/superman.png",
                    "price": "$2.99",
                    "series": "Batgirl",
                    "type": "comic book"
                },
                {
                    "thumb": "https://i.ibb.co/GCN80gY/superman.png",
                    "price": "$3.99",
                    "series": "Batman",
                    "type": "comic book"
                },
                {
                    "thumb": "https://i.ibb.co/GCN80gY/superman.png",
                    "price": "$2.99",
                    "series": "Batman Beyond",
                    "type": "comic book"
                },
                {
                    "thumb": "https://i.ibb.co/GCN80gY/superman.png",
                    "price": "$3.99",
                    "series": "Batman/Superman",
                    "type": "comic book"
                },
                {
                    "thumb": "https://i.ibb.co/GCN80gY/superman.png",
                    "price": "$4.99",
                    "series": "Batman/Superman Annual",
                    "type": "comic book"
                },
                {
                    "thumb": "https://i.ibb.co/GCN80gY/superman.png",
                    "price": "$5.99",
                    "series": "Batman: The Joker War Zone",
                    "type": "comic book"
                },
                {
                    "thumb": "https://i.ibb.co/GCN80gY/superman.png",
                    "price": "$6.99",
                    "series": "Batman: Three Jokers",
                    "type": "comic book"
                },
                {
                    "thumb": "https://i.ibb.co/GCN80gY/superman.png",
                    "price": "$4.99",
                    "series": "Batman: White Knight Presents: Harley Quinn",
                    "type": "comic book"
                },
                {
                    "thumb": "https://i.ibb.co/GCN80gY/superman.png",
                    "price": "$16.99",
                    "series": "Catwoman",
                    "type": "graphic novel"
                }
            ]
        }
    }
}
</script>

<!-- PARTE HTML -->
<template>
    <section class="cards_section">
        <div class="cards_container">
            <div v-for="comics in cards">
                <ItemCardsModel v-bind:img="comics.thumb" v-bind:title="comics.series.toUpperCase()" />
            </div>
        </div>
        <button type="button">LOAD MORE</button>
        <button id="special_btn">CURRENT SERIES</button>
    </section>
</template>

<!-- PARTE SCSS-->
<style lang="scss"> //rimosso lo scoped da <style> per ereditare la classe "card" del modello component ItemCardsModel
 @use '../assets/styles/partials/variables' as *;

 .cards_section {
     display: flex;
     flex-direction: column;
     position: relative;

     button {
         align-self: center;
         background-color: $text_second_color;
         color: $text_first_color;
         font-weight: bold;
         padding: .9375rem 3.125rem;
         margin: 2.5rem 0 1.25rem 0;
         border: none;
         cursor: pointer;
     }

     #special_btn {
         position: absolute;
         font-size: 1.125rem;
         top: -70px;
         left: 0px;
         padding: .9375rem 1.875rem;
     }

 }

 .cards_container {
     display: flex;
     justify-content: space-between;
     flex-wrap: wrap;

     .card {
         margin-top: 3.125rem;
         margin-bottom: .625rem;
         width: 11.25rem;
         height: 11.25rem;

         img {
             width: 100%;
         }
     }

     h3 {
         font-size: .8125rem;
         width: 11.875rem;
         margin-bottom: 1.25rem;
     }
 }
</style>