<template>
    <div>
        <img src="../assets/img/jumbotron.jpg" alt="">
    </div>
</template>

<script>
export default {
    name: 'JumboTron',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
div {
    height: 350px;
    img {
        height: 100%;
        width: 100%;
        object-fit: cover;
        object-position: top;
    }
}
</style>