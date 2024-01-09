<template>
  <div class="main-app">
    <page-menu />
    <div class="main-app__content">
      <page-barnner />
      <my-skills />
    </div>
    <page-footer />
  </div>
</template>

<script>
import PageMenu from '@/components/PageMenu.vue';
import PageBarnner from '@/components/PageBarnner.vue';
import MySkills from '@/home/MySkills.vue';
import PageFooter from './components/PageFooter.vue';
export default {
  name: 'App',
  components: {
    PageMenu,
    PageBarnner,
    MySkills,
    PageFooter
    
  }
}
</script>

<style lang="scss" scoped>
@import url("@/components/_app.scss");
  *{
    margin: 0px;
    padding: 0px;
  }

  html,body{
    margin: 0px;
    padding: 0px;
  }
  .main-app{
    border: none;
    width: 100%;
    padding: 0px;
    background: transparent;
    &__content{
      border: none;
      width: 80%;
      margin: 0 auto;
      padding: 0px;
    }
  }
</style>
