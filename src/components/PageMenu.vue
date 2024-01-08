<template>
    <div class="main-menu">
        <div class="main-menu__logo">
            <div class="main-menu__logo__imglogo">
                <img src="../assets/logo.png" alt="" class="main-menu__logo__imglogo__logo" >
            </div>
            <div class="main-menu__logo__info">
                <p>Conteudos importantes e relevantes</p>
            </div>
        </div>
        <div class="main-menu__links">
            <a href="#" class="main-menu__links__link">Menu 1</a>
            <a href="#" class="main-menu__links__link">Menu 2</a>
            <a href="#" class="main-menu__links__link">Menu 3</a>
            <a href="#" class="main-menu__links__link">Menu 4</a>
        </div>
    </div>
</template>

<script>
    export default{
        name: "PageMenu"
    }
</script>

<style lang="scss" copped>
@import "@/components/app.scss";
    .main-menu{
        background: $color-white;
        padding: 10px 0px 1px 0px;
        width: 100%;
        &__logo{
             width: 100%;
             display: flex;
             justify-content: space-between;
             padding-bottom: 10px;
            &__imglogo{
                border: none;
                margin-left: 10px;
                width: 20%;
                &__logo{
                    width: 40px;
                    height: 40px;
                }
            }
            &__info{
                color: $color2;
                border:none;
                margin-right:10px;
                text-align: right;
                width: 70%;
                display: flex;
                align-items:last baseline;
                justify-content: flex-end;
            }
        }
        &__links{
            border: none;
            display: flex;
            justify-content: center;
            padding: 10px;
            background: $color2;
            &__link{
                text-decoration: none;
                color: $color6;
                font-family: $ff-secondary;
                font-size: 14px;
                font-weight: bold;
                margin: 10px;
            }
        }
    }
</style>