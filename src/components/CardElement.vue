<script>
export default {
    name: 'Card',
    props: {
        link: String,
        title: String
    }
}
</script>
<template>
    <div class="card">
        <div><img :src="link"></div>
        <h3>{{ title }}</h3>
    </div>
</template>
<style lang="scss" scoped>
h3 {
    margin-top: 20px;
}
</style>