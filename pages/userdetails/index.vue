<template lang="">
    <div class="bg-gray-200  h-full">
           <navbar/>
        <travelinfo/>
        <foot/>
    </div>
</template>
<script>
import travelinfo from '~/components/travelinfo';
import foot from '~/components/footer';
import navbar from '~/components/navbar';
export default {
    components:{
        travelinfo,
        foot,
        navbar
    }
}
</script>