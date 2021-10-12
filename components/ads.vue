<template>
    <div class="bg-gray-200 py-6 h-full">
      <div class="bg-white rounded py-3 px-3 w-48  shadow ">
          <div class="mb-2 border-b border-gray-400 py-3" v-for="ad in ads" :key="ad.body">
              <a href="#" class="flex items-center">
                  <img :src="ad.src" alt="">
                  <p class="text-blue-600 font-normal mx-2 text-sm">{{ad.site}}</p>
              </a>
              <p class="text-green-600 font-normal text-left text-sm  leading-tight tracking-tighter">{{ad.title}}</p>
              <p class="text-black leading-tight text-sm mt-2">{{ad.body}}</p>
          </div>
         <div>
             
        </div> 
      </div>
    </div>
</template>
<script>
export default {
    data() {
        return {
            ads:[
                { 
                    src: require("../static/ads/ka.png"),site:'kenya-airways.com',
                title:'Kenya Airways - Dubai - Fly Kenya Airways - Cameroon - Dubai - kenya-airways.com',
                body:'Experience African hospitality at its best. When you fly Kenya Airways, you are our guest.'
                },

                { 
                    src: require("../static/ads/trip.png"),site:'tripadvisor.com',
                title:'Cheap Flights from Douala to Dubai - Tripadvisor',
                body:'Cheap flights to all destinations. Search on Tripadvisor deals'
                },

                { 
                src: require("../static/ads/faviconV2.png"),site:'bravofly.no',
                title:'Douala Fly - Bestill flybilletter på farten - Fly verden rundt for mindre - bravofly.no',
                body:'Bravofly.no® – Søk, sammenlign og bestille flybillett på minutter. Bestill nå'
                },

                { 
                src: require("../static/ads/kiwi.png"),site:'kiwi.com',
                title:'Fly to Dubai - Fly Cheaply & Save Money - kiwi.com',
                body:'Travel to Dubai. Book Now To Get The Best Deal on Flights'
                }
            ]
        }
    },
}
</script>