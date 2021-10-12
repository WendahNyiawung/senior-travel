<template>
  
    <header>
        
    <!-- Require css -->
    <style>
    .scroll-hidden::-webkit-scrollbar {
        height: 0px;
        background: transparent; /* make scrollbar transparent */
    }
    </style>
       <Navbar/>

        <div class="showcase h-screen w-full bg-cover bg-center" style="background-image: url(https://cutt.ly/5kaR0j0);">
            <div class="flex items-center justify-center h-full w-full bg-gray-900 bg-opacity-50">
                <div class="text-center">
                    <h1 class="text-white text-2xl font-semibold capitalize md:text-3xl lg:text-6xl font-bold">Your Jurney Begins</h1>
                    <div class="flex flex-col lg:flex-row items-center bg-white rounded p-2 mt-4 rounded sm:w-full">
                        <form action="" class="flex flex-col lg:flex-row items-center justify-between">
                       <input type="search" class="py-2 mx-2 border border-gray-300 focus:border-green-500  rounded focus:outline-none px-2" placeholder="From example Douala">
                       <input type="text" class="py-2  mx-2 border border-gray-300 focus:border-green-500  rounded focus:outline-none px-2" placeholder="To example Dubai">
                       <input type="text" class="py-2  mx-2 border border-gray-300 focus:border-green-500  rounded focus:outline-none px-2" placeholder="Dapature" onfocus="(this.type = 'date')">
                       <select id="class" name="class" autocomplete="class" class="mt-1 block w-full py-2 px-3 border border-gray-300 bg-white rounded-md shadow-sm focus:outline-none focus:ring-indigo-500 focus:border-indigo-500 sm:text-sm">
                           <option>Economy</option>
                           <option>Business</option>
                       </select>
                    </form>
                    <button type="submit" class="rounded bg-green-500 px-4 py-2 mx-2 focus:outline-none text-white">
                        <nuxt-link to="./oneway">Search</nuxt-link>
                    </button>
                    </div>
                </div>
            </div>
        </div>
    </header>
</template>

<script>
import navbar from '~/components/navbar';
export default {
 components:{
     navbar
 }
}
</script>

<style>

</style>