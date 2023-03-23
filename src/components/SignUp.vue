<script>
export default {
    nome: 'SignUp',
    data() {
        return {
            socialList: [
                {
                    logo: '../public/footer-facebook.png',
                    link: '#'
                },
                {
                    logo: '../public/footer-twitter.png',
                    link: '#'
                },
                {
                    logo: '../public/footer-youtube.png',
                    link: '#'
                },
                {
                    logo: '../public/footer-pinterest.png',
                    link: '#'
                },
                {
                    logo: '../public/footer-periscope.png',
                    link: '#'
                }
            ]
        }
    }

}
</script>
<template>
    <div class="row">
        <div>
            <button>SIGN-UP NOW!</button>
            <div class="socials">
                <h3>FOLLOW US</h3>
                <ul>
                    <li v-for="social in socialList"><a :href="social.link"><img :src="social.logo" alt="social"></a></li>
                </ul>
            </div>
        </div>
    </div>
</template>
<style lang="scss" scoped>
@use '../styles/general.scss' as *;
@use '../styles/variables.scss' as *;

* {
    z-index: 100;
}

.row {
    background-color: #303030;
    padding: 30px 0;
    position: relative;

    &>div {
        @include my-container;
        display: flex;
        justify-content: space-between;
        align-items: center;
    }
}

button {
    border-radius: 0;
    background-color: transparent;
    border: 2px solid $dc-color;
    color: white;
    font-size: 16px;
    padding: 16px;
}

h3 {
    color: $dc-color;
}

.socials {
    display: flex;
    gap: 25px;
    align-items: center;
}

ul {
    list-style-type: none;
    display: flex;
    gap: 15px;
}
</style>