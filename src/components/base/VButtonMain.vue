<template>
    <div>
        <a href="#">
            {{ texto }}
        </a>
    </div>
</template>

<script>
    export default{
        name: "VButtonMain",
        props:{
            texto: String,
            colorTexto: String,
            colorFondo: String
        }
    }
</script>

<style lang="scss" scoped>

</style>