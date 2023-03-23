<script>
import LogoApp from './LogoApp.vue';
import NavDC from './NavDC.vue';
export default {
    nome: 'Header',
    components: {
        LogoApp,
        NavDC
    }
}
</script>
<template>
    <header>
        <!-- LOGO -->
        <LogoApp></LogoApp>
        <!-- /LOGO -->
        <!-- NAV -->
        <NavDC></NavDC>
        <!-- /NAV -->
    </header>
</template>
<style lang="scss" scoped>
@use '../styles/general.scss' as *;
@use '../styles/variables.scss' as *;

header {
    @include my-container;
    justify-content: space-between;
}
</style>
