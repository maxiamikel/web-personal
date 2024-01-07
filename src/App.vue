<template>
  <div>
    <personal-data />
    <about-me />
    <my-skills />
  </div>
</template>

<script>
import PersonalData from '@/home/PersonalData.vue';
import AboutMe from '@/home/AboutMe.vue';
import MySkills from '@/home/MySkills.vue';

export default {
  name: 'App',
  components: {
    PersonalData,
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
