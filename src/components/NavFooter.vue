<script>
export default {
    nome: 'NavFooter',
    data() {
        return {
            //ARRAY MENU
            shopLinks: [
                {
                    name: 'DIGITAL COMICS',
                    img: '../public/buy-comics-digital-comics.png',
                    link: '#'
                },
                {
                    name: 'DC MERCHANDISE',
                    img: '../public/buy-comics-merchandise.png',
                    link: '#'
                },
                {
                    name: 'SUBSCRIPTION',
                    img: '../public/buy-comics-subscriptions.png',
                    link: '#'
                },
                {
                    name: 'COMIC SHOP LOCATOR',
                    img: '../public/buy-comics-shop-locator.png',
                    link: '#'
                },
                {
                    name: 'DC POWER VISA',
                    img: '../public/buy-dc-power-visa.svg',
                    link: '#'
                }
            ]
        }
    }
}
</script>
<template>
    <div>
        <ul>
            <!-- NAV CREATED W/VUE -->
            <li v-for="shopLink in shopLinks"><a href="shopLink.link"><img :src="shopLink.img" alt="ciao">{{ shopLink.name
            }}</a></li>
        </ul>
    </div>
</template>
<style lang="scss" scoped>
@use '../styles/general.scss' as *;
@use '../styles/variables.scss' as *;

* {
    z-index: 100;
}

div {
    padding: 50px 0;
    background-color: $dc-color;
}

ul {
    @include my-container;
    display: flex;
    justify-content: space-around;
    list-style-type: none;
}


a {
    text-decoration: none;
    color: white;
    display: flex;
    align-items: center;
    gap: 15px;
}

img {
    height: 55px;
}
</style>