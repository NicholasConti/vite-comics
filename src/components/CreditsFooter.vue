<script>
export default {
    nome: 'Credits',
    data() {
        return {
            DcComicsList: [
                {
                    name: 'Characters',
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
                    name: 'Videos',
                    link: '#'
                },
                {
                    name: 'News',
                    link: '#'
                }
            ],
            DcList: [
                {
                    name: 'Term of use',
                    link: '#'
                },
                {
                    name: 'Privacy policy(New)',
                    link: '#'
                },
                {
                    name: 'Ad Choices',
                    link: '#'
                },
                {
                    name: 'Advertising',
                    link: '#'
                },
                {
                    name: 'Jobs',
                    link: '#'
                },
                {
                    name: 'Subscriptions',
                    link: '#'
                },
                {
                    name: 'Talent Workshops',
                    link: '#'
                },
                {
                    name: 'CPSC Certificates',
                    link: '#'
                },
                {
                    name: 'Ratings',
                    link: '#'
                },
                {
                    name: 'Shop Help',
                    link: '#'
                },
                {
                    name: 'Contact US',
                    link: '#'
                }
            ],
            sitesList: [
                {
                    name: 'DC',
                    link: '#'
                },
                {
                    name: 'MAD Magazine',
                    link: '#'
                },
                {
                    name: 'DC Kids',
                    link: '#'
                },
                {
                    name: 'DC Universe',
                    link: '#'
                },
                {
                    name: 'DC Power Visa',
                    link: '#'
                }
            ],
            ShopList: [
                {
                    name: 'Shop DC',
                    link: '#'
                },
                {
                    name: 'Shop DC Collectibless',
                    link: '#'
                }
            ],
        }
    }
}
</script>
<template>
    <div class="row">
        <div>
            <ul class="list-credits">
                <li class="title-credit">DC COMICS
                    <ul>
                        <li v-for="element in DcComicsList" class="subtitle"><a :href="element.link">{{ element.name }}</a>
                        </li>
                    </ul>
                </li>
                <li class="title-credit">SHOP
                    <ul>
                        <li v-for="element in ShopList" class="subtitle"><a :href="element.link">{{ element.name }}</a>
                        </li>
                    </ul>
                </li>
                <li class="title-credit">DC
                    <ul>
                        <li v-for="element in DcList" class="subtitle"><a :href="element.link">{{ element.name }}</a>
                        </li>
                    </ul>
                </li>
                <li class="title-credit">SITES
                    <ul>
                        <li v-for="element in sitesList" class="subtitle"><a :href="element.link">{{ element.name }}</a>
                        </li>
                    </ul>
                </li>


            </ul>
            <img src="../../public/dc-logo-bg.png" alt="">
        </div>
    </div>
</template>
<style lang="scss" scoped>
@use '../styles/general.scss' as *;

div.row {
    padding-top: 30px;
    background-image: url(../../public/footer-bg.jpg);
    background-size: cover;


    &>div {
        @include my-container;
        position: relative;
    }
}

img {
    position: absolute;
    z-index: 1;
    right: 0;
    bottom: 0;
    transform: translateY(+15%);
}

ul {
    list-style-type: none;
}

.list-credits {
    display: flex;
    height: 370px;
    flex-direction: column;
    flex-wrap: wrap;
}

.title-credit {
    color: white;
    font-size: 20px;
    font-weight: bold;
    margin-right: 20px;
}

li>ul {
    margin-top: 20px;
}

.subtitle {
    font-size: 16px;
    color: #959595;
    font-weight: 400;
    margin-bottom: 10px;

}

a {
    text-decoration: none;
    color: inherit;
}
</style>