<template>
   <div class="bg-gray-200 py-16 px-4 md:px-12">
           <p class="block text-3xl text-gray-800 dark:text-white font-bold text-center">Popular Destination</p>
           <p class="block text-md text-gray-800 dark:text-white font-semibold text-center mb-10">Find the best price on flights to our most popular destinations from airports across the World.</p>
       <div class="container mx-auto">
        <div class="grid grid-cols-1 sm:grid-cols-4 gap-3 gap-y-8">
        <div v-for="place in places" :key="place.city">
            
    <div class="max-w-xs bg-white dark:bg-gray-800 shadow-lg rounded-lg overflow-hidden mx-auto">
         <a class="px-3 py-1 bg-gray-700 text-gray-100 text-sm font-bold  hover:bg-gray-500 ml-auto z-10 relative">{{ place.price}}</a>
        <img class="w-full h-56 object-cover -mt-6 transition duration-500 ease-in-out transform hover:-translate-y-1 hover:scale-110" :src="place.src" alt="city">
        
        <div class="py-2 px-3">
            <p class="block text-2xl text-gray-800 dark:text-white font-bold">{{ place.city}}</p>
            <span class="text-sm text-gray-700 dark:text-gray-200">{{ place.country }}</span>
        </div>
    </div>
        </div>
    </div>
   </div>
   </div>
</template>
<script>
export default {
    data(){
       return{
            places:[
            {src:require('../static/places/buea.jpg'), city:'Buea', country:'Cameroon', price:'from $125'},
            {src:require('../static/places/bankok.jpg'), city:'Bankok', country:'Thailand', price:'from $325'},
            {src:require('../static/places/dubai.jpg'), city:'Dubai', country:'UAE', price:'from $423'},
            {src:require('../static/places/london.jpg'), city:'London', country:'Great Britain', price:'from $330'},
            {src:require('../static/places/manila.jpg'), city:'Manila', country:'Philpines', price:'from $325'},
            {src:require('../static/places/peru.jpg'), city:'machu picchu', country:'Peru', price:'from $325'},
            {src:require('../static/places/tallinn.jpg'), city:'Tallinn', country:'Estonia', price:'from $325'},
            {src:require('../static/places/vietnam.jpg'), city:'Hanoi', country:'Vietnam', price:'from $325'}
        ]
       }
    }
}
</script>