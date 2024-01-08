<template>
    <div class="skills-main">
        <div class="skills-main__content">
            <div class="skills-main__content__title">
                <h4>Project title</h4>
            </div>
            <div class="skills-main__content__details">
                <div class="skills-main__content__details__foto">
                    <img src="../assets/amikel.jpg" alt="Project title" class="skills-main__content__details__foto__image">
                </div>
                <div class="skills-main__content__details__description">
                    <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Esse reiciendis libero 
                        porro debitis, provident consequuntur quasi! Natus et, ipsam ad voluptatibus dolor 
                        doloremque labore, odit quasi dolorum possimus dolorem repellat.</p>
                        <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Esse reiciendis libero 
                        porro debitis, provident consequuntur quasi! Natus et, ipsam ad voluptatibus dolor 
                        doloremque labore, odit quasi dolorum possimus dolorem repellat.</p>
                        <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Esse reiciendis libero 
                        porro debitis, provident consequuntur quasi! Natus et, ipsam ad voluptatibus dolor 
                        doloremque labore, odit quasi dolorum possimus dolorem repellat.</p>
                </div>
            </div>
            <div class="skills-main__content__button">
                <v-button-main 
                    texto="Ver más" 
                    color-texto="#ff9f1a"
                    color-fondo="#212121"
                />
            </div>
        </div>
    </div>
</template>

<script>
import VButtonMain from '@/components/base/VButtonMain.vue';
    export default{
        name: "MySkills",
        components:{
            VButtonMain
        }
    }
</script>

<style lang="scss" scoped>
    @import "@/components/_app.scss";

    .skills-main{
        background: $color-white;
        border: solid 1px;
        &__content{
            width: 42%;
            border: solid 1px $color2;
            &__title{
                text-align: center;
                background: $color2;
                padding: 5px;
            }
            &__details{
                display: flex;
                &__foto{
                    width: 30%;
                    background: red;
                    &__image{
                        width: 100%;
                    }
                }
                &__description{
                    width: 70%;
                    text-align:left;
                    background: #333;
                }

            }
            &__button{
                border: solid1px blue;
                background: transparent;
                padding: 1px;
                text-align: center;
            }
        }
    }
</style>