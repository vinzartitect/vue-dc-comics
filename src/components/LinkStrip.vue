<template>
    <section class="link-strip">
        <img src="../assets/img/buy-comics-digital-comics.png" alt="">
        <ul>
            <li v-for="(link, i) in links" :key="i">
                <a :href="`${link.url}`">
                    <img :src="`../assets/img/${link.img}`" :alt="`${link.text}`">
                    {{link.text}}
                </a>
            </li>
        </ul>
    </section>
</template>

<script>
export default {
    name: 'LinkStrip',
    data(){
        return{
            links:[
                {
                    img: 'buy-comics-digital-comics.png',
                    text: 'DIGITAL COMICS',
                    url: '#',
                },
                {
                    img: 'buy-comics-merchandise.png',
                    text: 'DC MERCHANDISE',
                    url: '#',
                },
                {
                    img: 'buy-comics-subscriptions.png',
                    text: 'SUBSCRIPTION',
                    url: '#',
                },
                {
                    img: 'buy-comics-shop-locator.png',
                    text: 'COMIC SHOP LOCATOR',
                    url: '#',
                },
                {
                    img: 'buy-dc-power-visa.svg',
                    text: 'DC POWER VISA',
                    url: '#',
                },
            ]
        }
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    .link-strip {
        background-color: #0282f9;
        padding: 50px 0;
        ul {
            width: 75%;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            li {
                display: inline-block;
                a {
                    display: flex;
                    align-items: center;
                    color: white;
                    text-decoration: none;
                    img {
                        height: 60px;
                        margin-right: 20px;
                    }
                }
            }
        }
    }
</style>