<template>
    <footer>

        <FooterNav/>
        <FooterSocial/>          

    </footer>
</template>

<script>
import FooterNav from './FooterNav.vue';
import FooterSocial from './FooterSocial.vue';

export default {
    name: 'FooterComp',
    components: {
        FooterNav,
        FooterSocial
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

</style>