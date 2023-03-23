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
            ]
        }
    }
}
</script>

<template>
    <div>
        <h3>DC COMICS</h3>
        <ul>
            <li v-for="link in dcComicsLinks"><a href="#"> {{ link }}</a></li>
        </ul>

        <h3>SHOP</h3>
        <ul>
            <li v-for="link in shopLinks"><a href="#"> {{ link }}</a></li>
        </ul>
    </div>
</template>

<style lang="scss" scoped>
div {
    padding: .5rem;

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
            }
        }
    }
}
</style>