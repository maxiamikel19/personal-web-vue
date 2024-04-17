<template>
    <div class="skills">
        <h1 class="skills__title">My skills</h1>
        <p class="skills__text">
            Lorem ipsum dolor sit amet consectetur, adipisicing elit. Voluptas explicabo magni assumenda rem nesciunt quae repudiandae est! Rerum cupiditate est et, corporis adipisci vitae ipsam assumenda culpa veniam deleniti modi.
        </p>
        <div  class="skills__items">
            <div class="skills__items__item" v-for="s in skills" :key="s.id">
                <v-card-main
                    :title= "s.title "
                    :content="s.description"
                    :bgColor="s.bgcolor"
                />
            
            </div>
        </div>
    </div>
</template>

<script>
import VCardMain from "@/components/base/VCardMain.vue";
    export default {
        
        name:"MySkills",
        components:{
            VCardMain
        },
        data(){
            return{
                skills:[
                    {id: 0, title: 'title 1', description:'Mi primeira habilidade at molestias repellendus dignissimos? Facilis aliquam eligendi unde fugit? ', bgcolor:'#ff9f1a'},
                    {id: 1, title: 'title 1', description:'Mi  habilidade 2 loLorem ipsum dolor sit amet, consectetur adipisicing elit. ', bgcolor:'#18dcff'},
                    {id: 2, title: 'title 1', description:'Mi primeira habilidade 3 Rerum tempora cum rem voluptatem similique', bgcolor:'#c56cf0'},
                    {id: 3, title: 'title 1', description:'Mi primeira habilidade 4 Ad necessitatibus dolorem officiis accusamus, quasi blanditiis! ', bgcolor:'#3ae374'},
                ]
            }
        }
    }
</script>



 

<style lang="scss" scoped>
@import "../_app.scss";
    .skills{
        background: $color1;
        padding: 4em;
        display: flex;
        justify-content: center;
        align-items: center;
        flex-direction: column;
        margin-top: 1px;
        &__title{
            color: $white;
            font-family: $ff-primary;
            font-size: 24px;
            font-weight: 900;
            padding-bottom: 1em;
        }
        &__text{
            color: $white;
            font-family: $ff-secondary;
            font-size: 15px;
        }
        &__items{
            display: grid;
            grid-template-columns: 400px 400px;
            @media screen and (max-width:768px) {
                display: flex ;
                flex-direction: column;
                padding-top: 2em;
            }
        }
    }
</style>