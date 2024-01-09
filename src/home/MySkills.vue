<template>
    <div>
        <div class="skills">
          <div class="skills__box">
            <div class="skills__content">
                <div class="skills__content__left">
                    <img src="../assets/amikel.jpg" alt="" class="skills__content__left__img">
                </div>
            <div  class="skills__content__right">
                    <h4  class="skills__content__right__title">Amikel Maxi</h4>
                    <p  class="skills__content__right__text">
                        Lorem ipsum dolor sit amet consectetur adipisicing elit. Culpa adipisci expedita 
                        unde ratione reiciendis sapiente. Adipisci, exercitationem. Architecto distinctio
                        fuga ipsam, doloremque doloribus inventore? Ut nulla soluta velit eos ex?
                    </p>
                    <div  class="skills__content__right__button">
                        <v-button-main 
                        texto="Ver mais" 
                        color-texto="#ff9f1a"
                        color-fondo="#212121"
                    />
                    </div>
            </div>
            </div>
            <div class="skills__box__list">
                <h1 class="skills__box__list__title">Habilidades</h1>
                <div class="skills__box__list__itens">
                    
                    <ul>
                        <li>Habilidade 1 teste</li>
                        <li>Habilidade 1 teste</li>
                        <li>Habilidade 1 teste</li>
                        <li>Habilidade 1 teste</li>
                    </ul>
                </div>
            </div>
          </div>
            <div class="skills__socials">
                <div class="skills__socials__title">
                    <h4 class="skills__socials__title__text">Follow</h4>
                </div>
                <div class="skills__socials__links">
                    <a href="#" class="skills__socials__links__link">Facebook</a>
                    <a href="#" class="skills__socials__links__link">Twetter</a>
                    <a href="#" class="skills__socials__links__link">Instagram</a>
                    <a href="#" class="skills__socials__links__link">Linkedin</a>
                    <a href="#" class="skills__socials__links__link">Youtube</a>
                    <a href="#" class="skills__socials__links__link">Skype</a>
                </div>
            </div> 
        </div>

        <div class="project">
            <h2 class="project__title">Mis Habilidades</h2>
            <p class="project__description">Descripção das habilidades</p>
            <div class="project__items">
                <div class="project__items__item" v-for="skill in skills" :key="skill.id">
                    <v-card-main 
                        :title=" skill.title "
                        :content="skill.content"
                        :color="skill.color"
                        :language="skill.language"
                        :date="skill.date"
                    />
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import VButtonMain from '@/components/base/VButtonMain.vue';
import VCardMain from '@/components/base/VCardMain.vue';
    export default{
        name: "MySkills",
        components:{
            VButtonMain,
            VCardMain
        },
        data(){
                return{
                     skills:[
                        {'id':0, 'title':'Sistema de gestão', 'content':'Esse sistema es uma ferramenta para dinamizar e agilizar os processos de administração académicos','language':'Java/ Spring boot','date':'2021-10-10',color: "#AED6F1"},
                        {'id':1, 'title':'Sistema de administracao academico', 'content':'Esse sistema es uma ferramenta para dinamizar e agilizar os processos de administração académicos','language':'Java/ Spring boot','date':'2021-10-10',color:"#c56cf0"},
                        {'id':2, 'title':'Sistema de administracao academico', 'content':'Esse sistema es uma ferramenta para dinamizar e agilizar os processos de administração académicos','language':'Java/ Spring boot','date':'2021-10-10',color:"#c5621f"},
                        {'id':3, 'title':'Sistema de administracao academico', 'content':'Esse sistema es uma ferramenta para dinamizar e agilizar os processos de administração académicos','language':'Java/ Spring boot','date':'2021-10-10',color:"#0560ef"},
                        {'id':4, 'title':'Sistema de administracao academico', 'content':'Esse sistema es uma ferramenta para dinamizar e agilizar os processos de administração académicos','language':'Java/ Spring boot','date':'2021-10-10',color:"#0560ef"}
                    ]
                }   
            }
    }
</script>

<style lang="scss" scoped>
    @import "@/components/_app.scss";

    .skills{
        display: block;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        padding: 3em 4em 3em 4em;
        background: $color2;
        opacity: 0.5em;
        border: none;
        &__content{
            display: flex;
            justify-content: center;
            align-items: center;
            width: 45%;
            border: solid 1px $color6;
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
        &__box{
            border: none;
            display: flex;
            justify-content:space-around;
            align-items: center;
            &__list{
                display: block;
                border: solid 1px $color6;
                width: 40%;
                color: $color-white;
                align-items: center;
                justify-content:center;
                flex-direction: column;
                &__title{
                    font-size: 15px;
                    font-family: $ff-secondary;
                    border-bottom: solid 1px $color6;
                    padding-bottom: 1em;
                    margin:1.2em 0.3em 2em 0em;
                    text-align: left;
                    float: right;
                    width:70%;
                }
                &__itens{
                    border: none;
                    margin: 60px;
                    &__item{
                        margin-bottom: 3px;
                        font-family: $ff-primary;
                        font-weight: normal;
                    }
                }

            }
        }
        &__socials{
                background:transparent;
                border: none;
                width: 100%;
                margin: 10px 0px 0px 0px;
                display: block;
                justify-content: flex-end;
                align-items: center;
                &__title{
                    border: none;
                    &__text{
                        color: red;
                        text-align: right;
                    }
                }
                &__links{
                    border:none;
                    text-align: right;
                    &__link{
                       text-decoration: none;
                       color: $color6;
                       margin-left: 12px; 
                    }
                    
                }
            }
        
    }

    .project{
        border:none;
        margin-top: 10px;
        display: flex;
        align-items: center;
        flex-direction: column;
        justify-content: center;
        padding: 1em 1em 10em 1em;
        &__title{
            color: $color2;
            font-size: 15px;
            font-family: $ff-roboto;
        }
        &__description{
            font-family: $ff-secondary;
            font-size: 14px;
        }
        &__items{
            display: grid;
            grid-template-columns: 400px 400px;
        }
    }
</style>
