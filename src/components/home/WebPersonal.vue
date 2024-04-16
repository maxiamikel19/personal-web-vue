<template>
    <div class="personal-data">
        <div class="personal-data__left">
            <span class="personal-data__left__text">Ola</span>
            <h2 class="personal-data__left__name">Sou Amikel Maxi</h2>
            <p class="personal-data__left__text">
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Exercitationem, rem. Minus quo officiis qui dolorum unde natus ea, suscipit recusandae quas doloremque, vero maxime. Facere modi recusandae tempora dolorum ratione.
            </p>
            <v-button-main 
                text="Ver mais"
            />
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
</style>