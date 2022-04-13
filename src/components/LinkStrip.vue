<template>
    <section class="link-strip">        
        <ul>
            <!-- <li>
                <a>
                    <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                    <p>DIGITAL COMICS</p>
                </a>
            </li>
            <li>
                <a>
                    <img src="../assets/img/buy-comics-merchandise.png" alt="">
                    <p>DC MERCHANDISE</p>
                </a>
            </li>
            <li>
                <a>
                    <img src="../assets/img/buy-comics-subscriptions.png" alt="">
                    <p>SUBSCRIPTION</p>
                </a>
            </li>
            <li>
                <a>
                    <img src="../assets/img/buy-comics-shop-locator.png" alt="">
                    <p>COMIC SHOP LOCATOR</p>
                </a>
            </li>
            <li>
                <a>
                    <img src="../assets/img/buy-dc-power-visa.svg" alt="">
                    <p>DC POWER VISA</p>
                </a>
            </li> -->
            <li v-for="(link, i) in links" :key="i">
                <a :href="`${link.url}`">
                    <img :src="require(`../assets/img/${link.img}`)" :alt="`${link.text}`">
                    <p>{{link.text}}</p>
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
                    cursor: pointer;
                    &:hover {
                        img{
                            transform: scale(1.1);
                        }
                        p {
                            text-decoration: underline;
                        }
                    }
                    img {
                        height: 50px;
                        margin-right: 10px;
                    }
                }
            }
        }
    }
</style>