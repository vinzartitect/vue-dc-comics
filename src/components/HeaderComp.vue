<template>
    <header>
        <a href="">
            <img src="../assets/img/dc-logo.png" alt="DC Logo">
        </a>
        <ul>
            <li v-for="link, i in links" :key="i" :class="link.here ? 'active' : '' ">
                <a :href="link.url">{{link.text}}</a>
            </li>
        </ul>
    </header>
</template>

<script>
export default {
    name: 'HeaderComp',
    data(){
        return{
            links: [
                {
                    text: 'CHARACTERS',
                    url: '#',
                    here: false,
                },
                {
                    text: 'COMICS',
                    url: '#',
                    here: true,
                },
                {
                    text: 'MOVIES',
                    url: '#',
                    here: false,
                },
                {
                    text: 'TV',
                    url: '#',
                    here: false,
                },
                {
                    text: 'GAMES',
                    url: '#',
                    here: false,
                },
                {
                    text: 'COLLECTIBLES',
                    url: '#',
                    here: false,
                },
                {
                    text: 'VIDEOS',
                    url: '#',
                    here: false,
                },
                {
                    text: 'FANS',
                    url: '#',
                    here: false,
                },
                {
                    text: 'NEWS',
                    url: '#',
                    here: false,
                },
                {
                    text: 'SHOP',
                    url: '#',
                    here: false,
                },
            ]
        }
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 80%;
    margin: 0 auto;
    img {
        padding: 20px 0;
    }
    li {
        display: inline-block;
        margin: 0 15px;
        transition: all .15s ease;
        padding: 62px 0;
        a {
            padding: 62px 0;
            text-decoration: none;
            color: black;
            font-weight: bold;
        }
        &.active {
            a {
                color: #0282f9;
            }
            border-bottom: 5px solid #0282f9;
        }
        &:hover {
            a {
                color: #0282f9;
            }
            border-bottom: 5px solid #0282f9;
        }
    }
}
</style>