<script>
export default {
    name: "FooterLinks",
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
            <div>
                <h3>DC COMICS</h3>
                <ul>
                    <li v-for="link in dcComicsLinks"><a href="#"> {{ link }}</a></li>
                </ul>
            </div>

            <div>
                <h3>SHOP</h3>
                <ul>
                    <li v-for="link in shopLinks"><a href="#"> {{ link }}</a></li>
                </ul>
            </div>

        </div>
        <div class="right">
            <div>
                <h3>DC</h3>
                <ul>
                    <li v-for="link in dcLinks"><a href="#"> {{ link }}</a></li>
                </ul>
            </div>
            <div>
                <h3>SHOP</h3>
                <ul>
                    <li v-for="link in shopLinks"><a href="#"> {{ link }}</a></li>
                </ul>
            </div>

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