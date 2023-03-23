<script>

export default {
    name: 'Features',
    data() {
        return {
            features: [
                {
                    icon: '/features-icons/buy-comics-digital-comics.png',
                    text: 'Digital Comics'
                },
                {
                    icon: '/features-icons/buy-comics-merchandise.png',
                    text: 'DC Merchandise'
                },
                {
                    icon: '/features-icons/buy-comics-subscriptions.png',
                    text: 'Subscription'
                },
                {
                    icon: '/features-icons/buy-comics-shop-locator.png',
                    text: 'Comics Shop Locator'
                },
                {
                    icon: '/features-icons/buy-dc-power-visa.svg',
                    text: 'DC Power Visa'
                }
            ]
        }
    }
}
</script>

<template>
    <section>
        <div v-for="feature in features">
            <img :src="feature.icon" alt="">
            <h4>{{ feature.text.toUpperCase() }}</h4>
        </div>
    </section>
</template>

<style lang="scss">
section {
    background-color: #0782fa;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;

    div {
        display: flex;
        align-items: center;
        color: white;
        padding: 1rem;

        h4 {
            font-size: .8125rem;
        }

        img {
            width: 3.125rem;
        }
    }
}
</style>