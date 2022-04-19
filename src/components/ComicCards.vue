<template>
    <div class="comic-card">
        <a href="">
            <img class="comic-cover" :src="details.thumb" :alt="details.series">
            <span class="comic-title">{{details.series}}</span>
        </a>
    </div>
</template>

<script>
export default {
    name: 'ComicCards',
    props: {
        details: Object,
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    .comic-card {
        a {
            text-decoration: none;
        }
        width: calc(100% / 6);
        padding: 0 20px;
        margin-bottom: 50px;
        transition: all .1s ease;
        color: white;
        &:hover {
            transform: scale(1.02);
        }
        .comic-cover {
            width: 100%;
            display: block;
            aspect-ratio: 1;
            object-fit: cover;
            object-position: top;
            margin-bottom: 15px;
        }
        .comic-title {
            color: white;
            font-size: 12px;
            text-transform: uppercase;
        }
    }
</style>