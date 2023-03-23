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
nav {
    display: flex;
    flex-wrap: wrap;
    margin-left: .625rem;

    a {
    text-decoration: none;
    color: #464648;
    padding: .875rem;
    font-weight: bold;

    &:hover {
        color: #0782fa;
        box-shadow: 0 .25rem 0 #0782fa;
    }
}
}
</style>