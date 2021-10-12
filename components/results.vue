<template>
  <div>
    
    <div class="bg-gray-200 h-full py-6 mx-6">
      <div v-for="result in results" :key="result.destination" class="py-2">
        <div
          class="max-w-2xl mx-auto px-8 py-4 bg-white dark:bg-gray-800 rounded-lg shadow-md"
        >
          <div class="flex flex-col items-start">
            <div class="flex items-start justify-between">
              <div class="flex items-start justify-between flex-1">
                <div class="flex items-center">
                  <img :src="result.src" alt="" class="h-8 object-cover" />
                  <div class="flex flex-col items-start ml-3">
                    <p class="text-gray-800 font-medium">{{ result.time }}</p>
                    <span class="text-gray-500 text-xs">{{
                      result.destination
                    }}</span>
                  </div>
                </div>
                <div class="flex flex-col items-start mx-6">
                  <p class="text-gray-800 font-medium">{{ result.stops }}</p>
                  <span class="text-gray-500 text-xs">{{
                    result.stoplocation
                  }}</span>
                </div>
                <div class="flex flex-col items-start mx-6">
                  <p class="text-gray-800 font-medium">{{ result.duration }}</p>
                </div>
              </div>
              <div class="border-l border-gray-500 px-2 flex flex-col items-start justify-around">
                  <p class="text-gray-900 font-semibold">{{result.price}}</p>
                  <nuxt-link to="userdetails" class="bg-green-300 border border-green-400 rounded text-green-600 px-3 PY-5 mt-5">Book Now</nuxt-link>
              </div>
            </div>
            <span class="text-gray-500 text-xs">{{ result.company }}</span>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
//import navbar from "~/components/navbar";
import ads from "~/components/ads";
export default {
  components: {
    //navbar,
    ads
  },

  data() {
    return {
      results: [
        {
          src: require("../static/airlines/ET.png"),
          time: "14:00 - 04:30",
          destination: "(DLA) Douala - (DXB) Dubai Intl",
          stops: "1 Stop",
          stoplocation: "ADD",
          duration: "11h 30m",
          price: "$413",
          company: "Ethopian Air"
        },
        {
          src: require("../static/airlines/TK.png"),
          time: "00:40 - 03:50",
          destination: "(DLA) Douala - (DXB) Dubai Intl",
          stops: "2 Stops",
          stoplocation: "NSI,IST",
          duration: "24h 10m",
          price: "$375",
          company: "Turkish Airlines"
        },
        {
          src: require("../static/airlines/ET.png"),
          time: "00:40 - 03:50",
          destination: "(DLA) Douala - (DXB) Dubai Intl",
          stops: "1 Stop",
          stoplocation: "ADD",
          duration: "24h 10m",
          price: "$375",
          company: "Ethopian Air"
        },
        {
          src: require("../static/airlines/ET.png"),
          time: "00:40 - 03:50",
          destination: "(DLA) Douala - (DXB) Dubai Intl",
          stops: "1 Stop",
          stoplocation: "ADD",
          duration: "24h 10m",
          price: "$375",
          company: "Ethopian Air"
        },
        {
          src: require("../static/airlines/KQ.png"),
          time: "00:40 - 03:50",
          destination: "(DLA) Douala - (DXB) Dubai Intl",
          stops: "2 Stops",
          stoplocation: "NSI,NRB",
          duration: "24h 10m",
          price: "$375",
          company: "Kenya Airways"
        },
        {
          src: require("../static/airlines/KP.png"),
          time: "00:40 - 03:50",
          destination: "(DLA) Douala - (DXB) Dubai Intl",
          stops: "2 Stops",
          stoplocation: "NSI,ADB",
          duration: "24h 10m",
          price: "$375",
          company: "ASKY"
        }
      ]
    };
  }
};
</script>
