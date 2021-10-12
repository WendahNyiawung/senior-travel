<template>
   <div class="">
      <Navbar/>
     <div class="bg-gray-200 py-12 h-screen">
        <div class="container mx-auto flex items-center justify-center">
             <div class="bg-white rounded py-5 px-3 shadow w-1/4">
                   <div class="">
                           <label for="" class="block tracking-wide w-full text-gray-600 text-sm mb-2">Email</label>
                           <input type="email" placeholder="enter your email" class="w-full px-2 py-2 border border-gray-400 rounded">
                    </div>
                   <div class="mt-3">
                           <label for="" class="block tracking-wide w-full text-gray-600 text-sm mb-2">Password</label>
                           <input type="password" placeholder="enter your password" class="w-full px-2 py-2 border border-gray-400 rounded">
                    </div>
                    <button type="submit" class="bg-green-400 px-4 py-2 mt-5 block w-full rounded text-white">
                        <nuxt-link to="oneway">Login</nuxt-link>
                    </button>
             </div>
        </div>
     </div>
   </div>
</template>
<script>
import navbar from '~/components/navbar'
export default {
    components:{
        navbar
    }
}
</script>