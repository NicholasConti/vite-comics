<script>
import JumbotronDc from './JumbotronDc.vue';
import CardsDC from './CardsDC.vue';
export default {
    nome: 'Main',
    components: {
        JumbotronDc,
        CardsDC
    }
}
</script>
<template>
    <main>
        <JumbotronDc></JumbotronDc>
        <CardsDC></CardsDC>
    </main>
</template>
<style lang="scss" scoped></style>
