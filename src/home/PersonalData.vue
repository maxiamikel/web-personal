<template>
    <div class="personal-data">
        <div class="personal-data__left">
            <span class="personal-data__left__text">Hola</span>
            <h4 class="personal-data__left__name">Mi nombre es Amikel Maxi</h4>
            <p class="personal-data__left__descriotion">Lorem ipsum dolor sit amet consectetur, adipisicing elit. Necessitatibus amet</p>
            <v-button-main texto="Contactar"/>
        </div>
        <div class="personal-data__right">
            <img src="../assets/amikel.jpg" class="personal-data__right__foto" alt="" />
        </div>
    </div>
</template>

<script>
    import VButtonMain from "@/components/base/VButtonMain.vue"
    export default{
        name:"PersonalData",
        components:{
            VButtonMain
        }
    }

</script>

<style lang="scss" scoped>
    @import "@/components/app.scss";

    .personal-data{
        border: solid 1px;
        display: flex;
    }
</style>