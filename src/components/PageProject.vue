<template>
    <div class="project">
        <div class="project__content">
            <div class="project__content__left">
                <img src="../assets/amikel.jpg" alt="" class="project__content__left__img">
            </div>
           <div  class="project__content__right">
                <h4  class="project__content__right__title">Titulo do projeto</h4>
                <p  class="project__content__right__text">
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Culpa adipisci expedita 
                    unde ratione reiciendis sapiente. Adipisci, exercitationem. Architecto distinctio
                     fuga ipsam, doloremque doloribus inventore? Ut nulla soluta velit eos ex?
                </p>
                <div  class="project__content__right__button">
                    <v-button-main 
                    texto="Ver mais" 
                    color-texto="#ff9f1a"
                    color-fondo="#212121"
                />
                
                </div>
           </div>
        </div>
    </div>
</template>

<script>
import VButtonMain from './base/VButtonMain.vue';
    export default{
        name:"PageProject",
        components:{
            VButtonMain
        }
    }
</script>

<style lang="scss" scoped>
     @import "@/components/_app.scss";

.project{
    border: none;
    &__content{
        display: flex;
        justify-content: center;
        align-items: center;
        width: 45%;
        &__left{
            border: solid 1px $color6;
            width: 150px;
            height: 200px;
            margin-right: 3em;
            &__img{
                width: 100%;
                position: relative;
                left: 10px;
                top: -10px;
            }
        }
        &__right{
            display: block;
            width: 50%;
            color: $color-white;
            &__title{
                font-size: 15px;
                font-family: $ff-secondary;
                border-bottom: solid 1px $color6;
                padding-bottom: 1em;
                margin-bottom: 1em;
            }
            &__text{
                margin-bottom: 1em;
                font-size: 14px;
                font-family: $ff-primary;
                font-weight: normal;
            }
        }
    }
    
}
</style>