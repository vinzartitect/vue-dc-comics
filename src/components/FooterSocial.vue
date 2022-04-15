<template>

        <div class="bg-container">
            <div class="link-cont">
                <a class="sign-btn" href="">SIGN-UP NOW!</a>
                <div>
                    <a href="">FOLLOW US</a>
                    <ul>
                        <li v-for="link, i in socialLinks" :key="i">
                            <a :href="link.url">
                                <img :src="require(`../assets/img/${link.img}`)" :alt="link.alt">
                            </a>
                        </li>
                    </ul>
                </div>
            </div>
        </div>

</template>

<script>
export default {
    name: 'FooterSocial',
    data(){
        return{
            socialLinks: [
                {
                    img: 'footer-facebook.png',
                    url: '#',
                    alt: 'Facebook'
                },
                {
                    img: 'footer-twitter.png',
                    url: '#',
                    alt: 'Twitter'
                },
                {
                    img: 'footer-youtube.png',
                    url: '#',
                    alt: 'YouTube'
                },
                {
                    img: 'footer-pinterest.png',
                    url: '#',
                    alt: 'Pinterest'
                },
                {
                    img: 'footer-periscope.png',
                    url: '#',
                    alt: 'Periscope'
                },
            ]
        }
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    .bg-container {
        background-color: #303030;
        .link-cont {
            width: 80%;
            margin: 0 auto;
            padding: 50px 0;
            display: flex;
            justify-content: space-between;
            .sign-btn {
                border: 2px solid #0282f9;
                padding: 15px;
                color: white;
                text-decoration: none;
                transition: all .2s ease;
                &:hover {
                    background-color: #0282f9;
                }
            }
            div {
                display: flex;
                align-items: center;
                > a {
                    color: #0282f9;
                    text-decoration: none;
                    font-weight: bold;
                    font-size: 1.3rem;
                    margin-right: 20px;
                }
                li {
                    display: inline-block;
                    margin-right: 10px;
                }
            }
        }
    }
</style>