<template>
    <div>
        <a href="" 
            class="main-btn"
            :style="{background:backgroundColor, color:textColor}"
        >
            {{ text }}
        </a>
    </div>
</template>

<script>
    export default {
        name:"VButtonMain",
        props:{

            text: String,
            textColor: String,
            backgroundColor: String
        }
    }
</script>

<style lang="scss" scoped>
@import '../_app.scss';
    .main-btn{
        padding: 10px 20px 10px 20px;
        border: solid 1px $color2;
        border-radius: 6px;
        text-decoration: none;
        margin-top: 10px;
    }
</style>