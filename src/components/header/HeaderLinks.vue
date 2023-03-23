<script>
export default {
    name: 'HeaderLinks',
    data() {
        return {
            links:
                [
                    {
                        destination: 'Characters',
                        href: '#'
                    },
                    {
                        destination: 'Comics',
                        href: '#'
                    },
                    {
                        destination: 'Movies',
                        href: '#'
                    },
                    {
                        destination: 'Tv',
                        href: '#'
                    },
                    {
                        destination: 'Games',
                        href: '#'
                    },
                    {
                        destination: 'Collectibles',
                        href: '#'
                    },
                    {
                        destination: 'Videos',
                        href: '#'
                    },
                    {
                        destination: 'Fans',
                        href: '#'
                    },
                    {
                        destination: 'News',
                        href: '#'
                    },
                    {
                        destination: 'Shop',
                        href: '#'
                    }
                ]
        }
    }
}

</script>

<template>
    <nav>
        <a v-for="link in links" :href="link.href">{{ link.destination.toUpperCase() }}</a>
    </nav>
</template>

<style lang="scss">
@use '../../styles/colors.scss' as *;

nav {
    display: flex;
    flex-wrap: wrap;
    margin-left: 1rem;

    a {
    text-decoration: none;
    color: #464648;
    padding: .875rem;
    font-weight: bold;

    &:hover {
        color: $primary-color;
        box-shadow: 0 .25rem 0 $primary-color;
    }
}
}
</style>