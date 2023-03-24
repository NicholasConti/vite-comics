<script>
import "@fontsource/montserrat";
import HeaderDcVue from './components/HeaderDc.vue';
import MainDC from './components/MainDC.vue';
import FooterDC from './components/FooterDC.vue';

export default {
    components: {
        HeaderDcVue,
        MainDC,
        FooterDC
    }
}
</script>

<template>
    <!-- HEADER -->
    <HeaderDcVue></HeaderDcVue>
    <!-- /HEADER -->
    <!-- MAIN -->
    <MainDC></MainDC>
    <!-- /MAIN -->
    <!-- FOOTER -->
    <FooterDC></FooterDC>
    <!-- /FOOTER -->
</template>

<style lang="scss">
@use './styles/variables.scss' as *;
@use './styles/general.scss' as *;
</style>
