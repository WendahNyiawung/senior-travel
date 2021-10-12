<template>
    <div>
        <div class="showcase mb-8">
            <div class="EU">
                  <button class="europe focus:outline-none" @click="showurope = !showurope">
                <svg viewBox="0 0 20 20" class="fill-current text-white h-8">
                    <path fillRule="evenodd" d="M5.05 4.05a7 7 0 119.9 9.9L10 18.9l-4.95-4.95a7 7 0 010-9.9zM10 11a2 2 0 100-4 2 2 0 000 4z" clipRule="evenodd" />
                </svg>
            </button>
            <div class="tooleurope bg-green-500 rounded shadow w-40 p-1" v-if="showurope">
                <p class="text-white text-center ">
                    Search for cheap Flights within Europe
                </p>
                <p class="text-center text-white"> <nuxt-link to="europe">Search Now</nuxt-link></p>
                   
              
            </div>
         </div>
         <div class="afri">
                  <button class="africa focus:outline-none" @click="show = !show">
                <svg viewBox="0 0 20 20" class="fill-current text-white h-8">
                    <path fillRule="evenodd" d="M5.05 4.05a7 7 0 119.9 9.9L10 18.9l-4.95-4.95a7 7 0 010-9.9zM10 11a2 2 0 100-4 2 2 0 000 4z" clipRule="evenodd" />
                </svg>
            </button>
            <div class="toolafrica bg-green-500 rounded shadow w-40 p-1" v-if="show">
                <p class="text-white text-center ">
                    Search for cheap Flights within Africa
                </p>
                <p class="text-center text-white"> <nuxt-link to="africa">Search Now</nuxt-link></p>
                   
              
            </div>
         </div>
         
        </div>
    </div>
</template>
<script>
export default {
    data(){
        return{
            show: false,
            showurope: false
        }
    }
}
</script>
<style  scoped>
   .showcase{
       background-image: url('~static/wrld-16.jpg');
       background-size: cover;
       height: 100vh;
       background-position:  center;
   }
   .africa{
       margin-top: 8rem !important; 
       margin-left: 43rem;
       z-index: 2;
   }
   .toolafrica{
       margin-left: 40rem;
   }
   .europe{
       margin-top: 13rem;
       margin-left: 45rem;
      
   }
   .tooleurope{
       margin-left: 42rem;
        z-index: 1;
   }
</style>>
    
</style>