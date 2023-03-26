<script>
import ComicsItem from './ComicsItem.vue';
import PrimaryButton from '../utility-view/PrimaryButton.vue';

export default {
    name: "ComicsList",
    components: {
        ComicsItem,
        PrimaryButton
    },
    data() {
        return {
            comics: [
                {
                    "thumb": "/comics/superman.jpg",
                    "price": "$19.99",
                    "series": "Action Comics",
                    "type": "comic book"
                },
                {
                    "thumb": "/comics/american-vampire.jpg",
                    "price": "$3.99",
                    "series": "American Vampire 1976",
                    "type": "comic book"
                },
                {
                    "thumb": "/comics/aquaman.jpg",
                    "price": "$16.99",
                    "series": "Aquaman",
                    "type": "graphic novel"
                },
                {
                    "thumb": "/comics/batgirl.jpg",
                    "price": "$2.99",
                    "series": "Batgirl",
                    "type": "comic book"
                },
                {
                    "thumb": "/comics/batman.webp",
                    "price": "$3.99",
                    "series": "Batman",
                    "type": "comic book"
                },
                {
                    "thumb": "/comics/batman2.jpg",
                    "price": "$2.99",
                    "series": "Batman Beyond",
                    "type": "comic book"
                },
                {
                    "thumb": "/comics/batman-superman.jpg",
                    "price": "$3.99",
                    "series": "Batman/Superman",
                    "type": "comic book"
                },
                {
                    "thumb": "/comics/batman-superman-annual.jpg",
                    "price": "$4.99",
                    "series": "Batman/Superman Annual",
                    "type": "comic book"
                },
                {
                    "thumb": "/comics/joker-warzone.jpg",
                    "price": "$5.99",
                    "series": "Batman: The Joker War Zone",
                    "type": "comic book"
                },
                {
                    "thumb": "/comics/joker2.webp",
                    "price": "$6.99",
                    "series": "Batman: Three Jokers",
                    "type": "comic book"
                },
                {
                    "thumb": "/comics/harley-quinn.webp",
                    "price": "$4.99",
                    "series": "Batman: White Knight Presents: Harley Quinn",
                    "type": "comic book"
                },
                {
                    "thumb": "/comics/catwoman.jpg",
                    "price": "$16.99",
                    "series": "Catwoman",
                    "type": "graphic novel"
                }
            ]
        }
    }
}
</script>

<template>
    <section>
        <div class="series">
            <PrimaryButton text="CURRENT SERIES"></PrimaryButton>
        </div>
        <div>
            <ComicsItem v-for="comic in comics" :image="comic.thumb" :title="comic.series"></ComicsItem>
        </div>
        <PrimaryButton text="LOAD MORE"></PrimaryButton>
    </section>
</template>

<style lang="scss" scoped>
section {
    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 10px;
    position: relative;



    .series {
        align-self: flex-start;
        position: absolute;
        top: -20px;
        left: 80px;

    }

    div {
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
    }
}
</style>