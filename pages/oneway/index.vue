<template>
    <div class="bg-gray-200">
        <navbar/>
        <div class="bg-gray-900 py-4 mt-5 container mx-auto w-2/4 rounded flex items-center justify-between px-4">
            <div class="">
                <p class="font-bold text-gray-400">Douala - Dubai</p>
                <p class="font-semibold text-gray-500">Monday 08, Feb | 1 Traveller</p>
            </div>  
            <button class="text-gray-900 rounded py-1 px-4 bg-white font-semibold">
                <nuxt-link to="/">Change</nuxt-link>
            </button>
        </div>
        <div class="flex items-start justify-center container mx-auto">
              <ads/>
              <results/>
        </div>
        <foot/>
    </div>
</template>
<script>
import results from '~/components/results';
import foot from '~/components/footer';
import ads from '~/components/ads';
import navbar from '~/components/navbar';
export default {
    components:{
        results,
        foot,
        ads,
        navbar
    }
}
</script>