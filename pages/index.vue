<template>
<div>
  <showcase/>
  <places/>
  <mapflight/>
  <foot/>
</div>
</template>

<script>
import showcase from '~/components/header';
import places from '~/components/popular';
import mapflight from '~/components/map';
import foot from '~/components/footer';


export default {
  components:{
    showcase,
    places,
    mapflight,
    foot
  }
}
</script>
<style 
   
  
</style>
