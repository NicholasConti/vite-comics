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
        <LogoApp></LogoApp>
        <NavDC></NavDC>
    </header>
</template>
<style lang="scss" scoped>
@use '../styles/general.scss' as *;
@use '../styles/variables.scss' as *;

header {
    @include my-container;
    padding: 20px 0;
    justify-content: space-between;
}
</style>
