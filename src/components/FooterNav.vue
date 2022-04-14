<template>

        <nav>
            <div class="container">
                <div class="link-cont">
                    <div>
                        <ul>
                            <h3>DC COMICS</h3>
                            <li v-for="link, i in dcComicsLinks" :key="i">
                                <a :href="link.url">{{link.text}}</a>
                            </li>
                        </ul>
                        <ul>
                            <h3>SHOP</h3>
                            <li v-for="link, i in shopLinks" :key="i">
                                <a :href="link.url">{{link.text}}</a>
                            </li>
                        </ul>
                    </div>
                    <ul>
                        <h3>DC</h3>
                        <li v-for="link, i in dcLinks" :key="i">
                            <a :href="link.url">{{link.text}}</a>
                        </li>
                    </ul>
                    <ul>
                        <h3>SITES</h3>
                        <li v-for="link, i in sitesLinks" :key="i">
                            <a :href="link.url">{{link.text}}</a>
                        </li>
                    </ul>
                </div>
                <img src="../assets/img/dc-logo-bg.png" alt="">
            </div>
        </nav>

</template>

<script>
export default {
    name: 'FooterNav',
    data(){
        return{
            dcComicsLinks: [
                {
                    url: '#',
                    text: 'Characters'
                },
                {
                    url: '#',
                    text: 'Comics'
                },
                {
                    url: '#',
                    text: 'Movies'
                },
                {
                    url: '#',
                    text: 'TV'
                },
                {
                    url: '#',
                    text: 'Games'
                },
                {
                    url: '#',
                    text: 'Videos'
                },
                {
                    url: '#',
                    text: 'News'
                },
            ],
            shopLinks: [
                {
                    url: '#',
                    text: 'Shop DC'
                },
                {
                    url: '#',
                    text: 'Shop DC Collectibles'
                },
            ],
            dcLinks: [
                {
                    url: '#',
                    text: 'Terms Of Use'
                },
                {
                    url: '#',
                    text: 'Privacy Policy (New)'
                },
                {
                    url: '#',
                    text: 'Ad Choices'
                },
                {
                    url: '#',
                    text: 'Advertising'
                },
                {
                    url: '#',
                    text: 'Jobs'
                },
                {
                    url: '#',
                    text: 'Subscriptions'
                },
                {
                    url: '#',
                    text: 'Talent Workshop'
                },
                {
                    url: '#',
                    text: 'CPSC Certificates'
                },
                {
                    url: '#',
                    text: 'Ratings'
                },
                {
                    url: '#',
                    text: 'Shop Help'
                },
                {
                    url: '#',
                    text: 'Contact Us'
                },
            ],
            sitesLinks: [
                {
                    url: '#',
                    text: 'DC'
                },
                {
                    url: '#',
                    text: 'MAD Magazine'
                },
                {
                    url: '#',
                    text: 'DC Kids'
                },
                {
                    url: '#',
                    text: 'DC Universe'
                },
                {
                    url: '#',
                    text: 'DC Power Visa'
                },
            ]           
        }
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    nav {
        background-image: url("../assets/img/footer-bg.jpg");
        // padding: 50px 0;
        color: white;
        .container {
            width: 80%;
            height: 400px;
            overflow: hidden;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            .link-cont {
                padding: 30px 0;
                display: flex;
                > * {
                    margin-right: 20px;
                }
                li {
                    list-style: none;
                        margin: 10px 0;
                        font-size: .8rem;
                    a {
                        color: gray;
                        text-decoration: none;
                        &:hover {
                            color: white;
                        }
                    }
                }
            }
            img {
                height: 150%;
                object-fit: cover;
                transform: translate(0, -20%);
            }
        }
    }
</style>