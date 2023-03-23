<script>
export default {
    nome: 'Main'
}
</script>
<template>
    <div>
        <main>
            <h1>CONTENT HERE</h1>
        </main>
    </div>
</template>
<style lang="scss" scoped>
@use '../styles/general.scss' as *;

div {
    padding: 50px 0;
    background-color: #1c1c1c;
}

main {
    @include my-container;
}

h1 {
    color: white;
    font-size: 40px;
}
</style>
