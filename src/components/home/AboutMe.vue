<template>
    <div class="about">
        <div class="about__content">
            <div class="about__content__left">
                <img src="../../assets/images/foto.svg" alt="" class="about__content__left__img">
            </div>
            <div class="about__content__right">
                <h3 class="about__content__right__title">Sobre mim</h3>
                <p class="about__content__right__description">
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Minus facere consequatur, iste ab facilis aperiam amet beatae architecto a pariatur rem illum numquam esse eaque impedit maiores sint sed placeat?
                </p>
                <div class="about__content__right__controls">
                    <v-button-main 
                        text="Github"
                        background-color="#212121"
                        text-color="#ff9f1a"
                    />

                    <v-button-main 
                        text="Linkedin"
                        background-color="#212121"
                        text-color="#ff9f1a"
                    />
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import VButtonMain from '@/components/base/VButtonMain.vue';
    export default {
        name:"AboutMe",
        components:{
            VButtonMain
        }
    }
</script>

<style lang="scss" scoped>
@import '../_app.scss';

    .about{
        @media screen and (max-width:768px) {
            display: block;
            padding: 2em;
        }
        display: flex;
        justify-content: center;
        align-items: center;
        padding-top: 5em;
        padding-bottom: 5em;
        background: $color1;
        margin-top: 1px;
        &__content{
            @media screen and (max-width:768px) {
            display: block;
            width: 100%;
            align-items: center;
            justify-content: center;
        }
            width: 70%;
            display: flex;
            align-items: center;
            justify-content: center;
            &__left{
                border: solid 1px $color2;
                width: 180px;
                height: 200px;
                margin-right: 3em;
                @media screen and (max-width:768px) {
                    width:130px;
                    height: 140px;
                    margin-bottom: 1em;
                    display: none;
                    &__img{
                        width: 80%;
                    }
                }
                &__img{
                    width: 100%;
                    height: 100%;
                    position: relative;
                    left: 18px;
                    top: -18px;
                    background: $white;
                }
            }
            &__right{
                display: block;
                width: 50%;
                color: $white;
                padding: 20px;
                @media screen and (max-width:768px) {
                    width: 80%;
                    padding: 2em;
                }
                &__title{
                    font-family: $ff-primary;
                    font-size: 17px;
                    font-weight: bold;
                    margin-bottom: 20px;
                    padding-bottom: 20px;
                    border-bottom: 2px solid $color2;
                }
                &__description{
                    font-family: $ff-secondary;
                    padding-bottom: 20px;
                    font-size: 14px;
                }
                &__controls{
                    display: flex;
                    padding-top: 10px;
                }
            }
        }
    }
</style>