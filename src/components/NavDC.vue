<script>
export default {
    nome: 'NavBar',
    data() {
        return {
            //MENU NAV
            linksNav: [
                {
                    name: 'Character',
                    link: '#'
                },
                {
                    name: 'Comics',
                    link: '#'
                },
                {
                    name: 'Movies',
                    link: '#'
                },
                {
                    name: 'TV',
                    link: '#'
                },
                {
                    name: 'Games',
                    link: '#'
                },
                {
                    name: 'Collectibles',
                    link: '#'
                },
                {
                    name: 'Videos',
                    link: '#'
                },
                {
                    name: 'Fans',
                    link: '#'
                },
                {
                    name: 'News',
                    link: '#'
                },
                {
                    name: 'Shop',
                    link: '#'
                }
            ]
        }
    }
}
</script>
<template>
    <ul>
        <!-- CICLE VUE -->
        <li v-for="link in linksNav"><a href="{{ link.link }}">{{ link.name }}</a></li>
    </ul>
</template>
<style lang="scss" scoped>
@use '../styles/variables.scss' as *;

ul {
    list-style-type: none;
    display: flex;
    align-items: center;
    gap: 30px;
    text-transform: uppercase;
}

li {
    height: 100%;
    line-height: 115px;

    &:hover {
        color: $dc-color;
        border-bottom: 5px solid $dc-color;
    }
}

a {
    text-decoration: none;
    color: inherit;
    font-weight: bold;
}
</style>