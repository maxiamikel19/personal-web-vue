<template>
    <div>
        <a href="">
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

</style>