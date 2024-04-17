<template>
    <div :style="{background: bgColor}" class="main-card">
        <h4 class="main-card__title">{{  title }}</h4>
        <p class="main-card__content">{{ content}}</p>
    </div>
</template>

<script>
    export default {
        name:"VCardMain",
        props:{
            title: String,
            content: String,
            bgColor:String
        }
    }
</script>

<style lang="scss" scoped>
@import '../_app.scss';
    .main-card{
        width:300px;
        padding: 2em;
        color: $white;
        margin: 10px;
        &__title{
            font-family: $ff-primary;
            font-size: 17px;
            margin-bottom: 15px;
            text-transform: capitalize;
        }
    }
</style>