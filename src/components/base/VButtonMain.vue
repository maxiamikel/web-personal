<template>
    <div class="main-btn">
        <a href="#" :style="{background:colorFondo, color:colorTexto}" class="main-btn__btn">
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
    @import "@/components/app.scss";
    .main-btn{
        margin: 10px 0px 10px 0px;
        padding: 10px 0px 2px 0px;
        &__btn{
            border: solid 1px $color2;
            padding: 7px 20px 7px 20px;
            text-decoration: none;
            border-radius: 10px;
        }
        
    }
</style>