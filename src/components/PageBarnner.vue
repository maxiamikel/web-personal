<template>
    <div class="barnner-main">
        <personal-data />
    </div>
</template>
<script>
import PersonalData from '@/home/PersonalData.vue';
    export default{
        name:"PageBarnner",
        components:{
            PersonalData
        }
    }
</script>
<style lang="scss" scoped>
    .barnner-main{
        height: 100%;
        width: 100%;
        margin: 0 auto;
    }
</style>