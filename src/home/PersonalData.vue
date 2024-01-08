<template>
    <div class="personal-data">
        <div class="personal-data__left">
           <div class="personal-data__left__content">
                <span class="personal-data__left__content__text">Hola</span>
                <h4 class="personal-data__left__content__name">Mi nombre es Amikel Maxi</h4>
                <p class="personal-data__left__content__description">Lorem ipsum dolor sit amet consectetur, adipisicing elit. Necessitatibus amet</p>
                <v-button-main 
                    texto="Contactar" 
                    color-texto="#ff9f1a"
                    color-fondo="#212121"
                />
           </div>
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
        border: none;
        display: flex;
        &__left{
            background: $color1;
            width: 60%;
            display: flex;
            align-items: center;
            justify-content: center;
            &__content{
                border: none;
                width: 300px;
                color: $color-white;
                &__text{
                    color: $color-white;
                    font-family: $ff-primary;
                    font-size: 16px;
                    margin-bottom: 10px;
                }
                &__name{
                    font-family: $ff-secondary;
                    font-weight: normal;
                    font-size: 17px;
                    margin-bottom: 10px;
                    margin-top: 10px;
                    color: $color2;
                }
                &__description{
                    font-size: 14px;
                    font-family: $ff-secondary;
                    margin-bottom: 13px;
                }
            }
        }
        &__right{
            background: $color2;
            width: 40%;
            &__foto{
                width:30%;
                position: relative;
            }
        }
    }
</style>