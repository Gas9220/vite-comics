<script>
import FeatureView from './FeatureView.vue';

export default {
    name: 'Features',
    components: {
        FeatureView
    },
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
        <div class="container">
            <div v-for="feature in features">
                <FeatureView :image="feature.icon" :text="feature.text"></FeatureView>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../../styles/colors.scss' as *;

section {
    background-color: $primary-color;

    div.container {
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        align-content: center;
    }
}
</style>