<template>
    <div :style="{background:color}" class="main-card">
        <div class="main-card__metadata">
            <div class="main-card__metadata__tecnology">
                <span>{{ language }}</span>
            </div>
            <div class="main-card__metadata__date">
                <span>{{date}}</span>
            </div>
        </div>
        <h3 class="main-card__title">{{ title }}</h3>
        <p class="main-card__text">{{ content }}</p>
    </div>
</template>

<script>
    export default{
        name: "VCardMain",
        props:{
            title: String,
            content: String,
            color: String,
            language:String,
            date: String
        }
    }
</script>

<style lang="scss" scoped>
@import "@/components/_app.scss";
    .main-card{
        width: 354px;
        height: 220px;
        padding: 1.0em;
        color: $color-white;
        margin-top: 10px;
        &__title{
            font-family: $ff-secondary;
            font-size: 20px;
            margin-bottom: 1em;
        }
        &__text{
            font-family: $ff-roboto;
            color: $color2;
        }
        &__metadata{
            width: 100%;
            background: transparent;
            display: flex;
            align-items: first baseline;
            justify-content: space-between;
            padding: 0px;
            &__tecnology{
                background:transparent;
                color: $color2;
                font-family: $ff-secondary;
                font-weight: bold;
                font-size: 10px;
                font-style: italic;
            }
            &__date{
                background:transparent;
                color: $color2;
                font-family: $ff-secondary;
                font-weight: bold;
                font-size: 10px;
                font-style: italic;
            }
        }

    }
</style>