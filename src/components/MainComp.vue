<template>
    <main>
        <JumboTron/>
        <!-- <ComicsBook/>            -->
    </main>
</template>

<script>
import JumboTron from '../components/JumboTron.vue'
// import ComicsBook from '../components/ComicsBook.vue'

export default {
    name: 'MainComp',
    components: {
        JumboTron,
        // ComicsBook,       
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
main {
    background-color: #000000;
    color: white;
    h1 {
        padding: 50px 15%;
    }
}
</style>