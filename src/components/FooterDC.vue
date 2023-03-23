<script>
import NavFooterVue from './NavFooter.vue';
import CreditsFooter from './CreditsFooter.vue';
import SignUp from './SignUp.vue';
export default {
    nome: 'Footer',
    components: {
        NavFooterVue,
        CreditsFooter,
        SignUp
    }
}
</script>
<template>
    <footer>
        <NavFooterVue></NavFooterVue>
        <CreditsFooter></CreditsFooter>
        <SignUp></SignUp>
    </footer>
</template>
<style lang="scss" scoped></style>