<script>
export default {
    name: "FooterLinksList",
    props: {
        listTitle: String,
        links: [String]
    }
}
</script>

<template>
    <div>
        <h3>{{ listTitle }}</h3>
        <ul>
            <li v-for="link in links"><a href="#"> {{ link }}</a></li>
        </ul>
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