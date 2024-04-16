<template>
  <div>
    <web-personal />
    <about-me />
    <my-skills />
  </div>
</template>

<script>
import WebPersonal from "@/components/home/WebPersonal.vue";
import AboutMe from "@/components/home/AboutMe.vue";
import MySkills from '@/components/home/MySkills.vue';

export default {
  name: 'App',
  components: {
    WebPersonal,
    AboutMe, 
    MySkills
  }
}
</script>

<style>
  *{
    margin: 0px;
    padding: 0px;
  }
</style>
