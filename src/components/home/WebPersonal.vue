<template>
    <div class="personal-data">
        <div class="personal-data__left">
            <div class="personal-data__left__content">
                 <span class="personal-data__left__content__text">Ola</span>
                <h2 class="personal-data__left__content__name">Sou Amikel Maxi</h2>
                <p class="personal-data__left__content__description">
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Exercitationem, rem. Minus quo officiis qui dolorum unde natus ea, suscipit recusandae quas doloremque, vero maxime. Facere modi recusandae tempora dolorum ratione.
                </p>
                <v-button-main 
                    text="Ver mais"
                    background-color="#212121"
                    text-color="#ff9f1a"
                />
            </div>
            
        </div>
        <div class="personal-data__right">
            <img src="../../assets/images/foto.svg" alt="" class="personal-data__right__img">
        </div>
    </div>
</template>

<script>
import VButtonMain from '@/components/base/VButtonMain.vue'
    export default {
        name:"WebPersonal",
        components:{

            VButtonMain
        }
    }
</script>

<style lang="scss" scoped>
@import '../_app.scss';
    .personal-data{
        display: flex;
        &__left{
            background: $color1;
            width: 60%;
            display: flex;
            justify-content: center;
            align-items: center;
            &__content{
                max-width: 60%;
                color: $white;
                &__text{
                    font-family: $ff-primary;
                    font-size: 14px;
                    font-weight: 700;
                    margin-bottom: 10px;
                }
                &__name{
                    font-family: $ff-secondary;
                    margin-bottom: 15px;
                    margin-top: 15px;
                    color: $color2;
                }
                &__description{
                    font-size: 15px;
                    font-family: $ff-secondary;
                    margin-bottom: 20px;
                }
            }
        }

        &__right{
            background: $color2;
            width: 40%;
            &__img{
                width:400px;
                position: relative;
            }   
        }
    }
</style>