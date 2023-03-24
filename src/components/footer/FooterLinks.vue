<script>
import FooterLinkList from './FooterLinkList.vue';

export default {
    name: "FooterLinks",
    components: {
        FooterLinkList
    },
    data() {
        return {
            dcComicsLinks: [
                "Characters",
                "Comics",
                "Movies",
                "TV",
                "Games",
                "Videos",
                "News"
            ],
            shopLinks: [
                "Shop DC",
                "Shop DC Collectibles"
            ],
            dcLinks: [
                "Terms Of Use",
                "Privacy Policy (New)",
                "Ad Choices",
                "Advertising",
                "Jobs",
                "Subscriptions",
                "Talent Workshops",
                "CPSC Certificates",
                "Ratings",
                "Shop Help",
                "Contact Us"
            ],
            sitesLinks: [
                "DC",
                "MAD Magazine",
                "DC Kids",
                "DC Universe",
                "DC Power Visa"
            ]
        }
    }
}
</script>

<template>
    <div class="links">
        <div class="left">
            <FooterLinkList listTitle = "DC COMIC" :links="dcComicsLinks"></FooterLinkList>
            <FooterLinkList listTitle = "SHOP" :links="shopLinks"></FooterLinkList>
        </div>
        <div class="right">
            <FooterLinkList listTitle = "DC" :links="dcLinks"></FooterLinkList>
            <FooterLinkList listTitle = "SHOP" :links="shopLinks"></FooterLinkList>
        </div>
    </div>
</template>

<style lang="scss" scoped>
div.links {
    display: flex;
    z-index: 2;

    div.right {
        display: flex;
    }

    div {
        margin-right: 15px;
        padding-bottom: 10px;

        h3 {
            color: white;
            margin-top: 15px;
        }

        ul {
            list-style-type: none;
            margin-top: .5rem;

            li {
                margin: .3125rem 0;

                a {
                    text-decoration: none;
                    color: gray;

                    &:hover {
                        color: white;
                    }
                }
            }
        }
    }
}
</style>