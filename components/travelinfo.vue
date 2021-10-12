<template>
    <div>
        <div class="py-6">
           <div class="bg-gray-900 py-2">
               <p class="text-center font-semibold text-lg text-gray-200">Who is Traveling?</p>
           </div>
           <div class="bg-white p-4 rounded shadow container mx-auto mt-4 w-2/3">
               <div class="border-l-4 border-green-400 mb-5">
                   <p class="text-gray-900 font-semibold ml-2">Personal Details</p>
               </div>
               <form action="">
                   <div class="flex items-center justify-evenly mb-5">
                       <div class="">
                           <label for="" class="block tracking-wide w-full text-gray-600 text-sm mb-2">First Name</label>
                           <input type="text" placeholder="Enter your First Name" class="px-2 py-1 border border-gray-400 rounded">
                       </div>
                       <div class="">
                           <label for="" class="block tracking-wide text-gray-600 text-sm mb-2">Last Name</label>
                           <input type="text" placeholder="Enter your Last Name" class="w-full px-2 py-1 border border-gray-400 rounded">
                       </div>
                       <div class="">
                           <label for="" class="block tracking-wide text-gray-600 text-sm mb-2">Date of birth</label>
                           <input type="date" placeholder="Enter your Last Name" class="px-2 py-1 w-full border border-gray-400 rounded">
                       </div>
                       <div class="">
                           <label for="" class="block tracking-wide text-gray-600 text-sm mb-2">Gender</label>
                            <select class="block appearance-none w-full  border border-gray-200 text-gray-700 py-2 px-4 pr-8 rounded leading-tight focus:outline-none focus:bg-white focus:border-gray-500" id="grid-state">
                             <option>Male</option>
                             <option>Female</option>
                             <option>other</option>
                            </select>
                       </div>
                   </div>
                   <div class="flex items-center justify-around">
                       <div class="">
                           <label for="" class="block tracking-wide w-full text-gray-600 text-sm mb-2">Nationality</label>
                           <input type="text" placeholder="Enter your Nationality" class="px-2 py-1 border border-gray-400 rounded">
                       </div>
                       <div class="">
                           <label for="" class="block tracking-wide text-gray-600 text-sm mb-2">Passport or ID Number</label>
                           <input type="number" placeholder="0000 0000 0000 0000" class="w-full px-2 py-1 border border-gray-400 rounded">
                       </div>
                       <div class="">
                           <label for="" class="block tracking-wide text-gray-600 text-sm mb-2">Expiry date</label>
                            <input type="number" placeholder="DD-MM-YYYY" class="w-full px-2 py-1 border border-gray-400 rounded">
                       </div>
                   </div>
                    <div class="border-l-4 border-green-400 mt-5">
                       <p class="text-gray-900 font-semibold ml-2">Baggage</p>
                    </div>
                    <div class="border border-gray-400 rounded px-8 py-4 mt-5">
                       <div class="flex items-center justify-between">
                         <p class="text-gray-900 font-semibold">Cabin Loggage</p>
                         <p class="text-gray-500 font-normal">42 X 22 X 40 cm</p>
                         <p class="text-gray-900 font-semibold">Free</p>
                       </div>
                       <div class="flex items-center justify-between mt-5">
                         <p class="text-gray-900 font-semibold">Checked Loggage</p>
                         <div class="flex items-center justify-between  border  border-gray-400 rounded py-2 px-2">
                            <p class="text-gray-500 font-semibold">{{ kg }}</p>  
                           <p class="text-gray-500 font-semibold mx-4">kg</p>
                           <div class="flex ">
                               <button @click="addPrice" class="focus:outline-none mx-4 bg-white hover:bg-gray-600 px-4  text-base hover:text-white">+</button>
                               <button @click="reducePrice" class="focus:outline-none mx-4 bg-white hover:bg-gray-600 px-4  text-base hover:text-white">-</button>
                           </div>
                         </div>
                         <p class="text-gray-900 font-semibold">$ <span class="">{{price}}</span></p>
                       </div>
                    </div>
                    <button type="submit" class="bg-green-400 py-2 px-4 rounded text-white mt-3">Add Passenger</button>
               </form>
           </div>
           <div class="container mx-auto my-6">
               <div class="bg-gray-900 py-2">
               <p class="text-center font-semibold text-lg text-gray-200">How will you like to pay?</p>
           </div>
           </div>
           <div class="bg-white p-4 rounded shadow container mx-auto mt-4 w-2/3">
               <div class="border-l-4 border-green-400 mb-5">
                   <p class="text-gray-900 font-semibold ml-2">Payment Details</p>
               </div>
               <form action="">
                   <div class="flex items-center justify-evenly mb-5">
                       <div class="">
                           <label for="" class="block tracking-wide w-full text-gray-600 text-sm mb-2">Card Number</label>
                           <input type="number" placeholder="0000 0000 0000 0000" class="px-2 py-1 border border-gray-400 rounded">
                       </div>
                       <div class="">
                           <label for="" class="block tracking-wide text-gray-600 text-sm mb-2">Name on Card</label>
                           <input type="text" placeholder=" name on Card" class="w-full px-2 py-1 border border-gray-400 rounded">
                       </div>
                       <div class="">
                           <label for="" class="block tracking-wide text-gray-600 text-sm mb-2">Expiry Date</label>
                           <input type="text" placeholder="MM / YY" class="px-2 py-1 w-full border border-gray-400 rounded">
                       </div>
                       <div class="">
                           <label for="" class="block tracking-wide text-gray-600 text-sm mb-2">CCV Code</label>
                             <input type="text" placeholder="CVV" class="px-2 py-1 w-full border border-gray-400 rounded">
                       </div>
                   </div>
                   <div class="flex items-center justify-evenly mb-5">
                       <div class="">
                           <label for="" class="block tracking-wide w-full text-gray-600 text-sm mb-2">Country</label>
                           <input type="number" placeholder="Country" class="px-2 py-1 border border-gray-400 rounded">
                       </div>
                       <div class="">
                           <label for="" class="block tracking-wide text-gray-600 text-sm mb-2">Billing Address</label>
                           <input type="text" placeholder=" Address" class="w-full px-2 py-1 border border-gray-400 rounded">
                       </div>
                       <div class="">
                           <label for="" class="block tracking-wide text-gray-600 text-sm mb-2">City</label>
                           <input type="text" placeholder="City" class="px-2 py-1 w-full border border-gray-400 rounded">
                       </div>
                       <div class="">
                           <label for="" class="block tracking-wide text-gray-600 text-sm mb-2">Zip Code</label>
                             <input type="text" placeholder="Zip Code" class="px-2 py-1 w-full border border-gray-400 rounded">
                       </div>
                   </div>
                   
                    <button type="submit" class="bg-green-400 py-2 px-4 rounded text-white mt-3">Submit</button>
               </form>
           </div>
           
           <div class="container mx-auto my-6">
               <div class="bg-gray-900 py-2">
               <p class="text-center font-semibold text-lg text-gray-200">Where should we send Confirmation?</p>
           </div>
           </div>
           <div class="bg-white p-4 rounded shadow container mx-auto mt-4 w-2/3">
               <div class="border-l-4 border-green-400 mb-5">
                   <p class="text-gray-900 font-semibold ml-2">Confirmation Details</p>
               </div>
               <form action="">
                   <div class="flex items-center justify-around mb-5">
                       <div class="">
                           <label for="" class="block tracking-wide w-full text-gray-600 text-sm mb-2">Email</label>
                           <input type="number" placeholder="Email" class="px-2 py-1 border border-gray-400 rounded">
                       </div>
                       <div class="">
                           <label for="" class="block tracking-wide text-gray-600 text-sm mb-2">Phone Number</label>
                           <input type="text" placeholder=" Phone Number" class="w-full px-2 py-1 border border-gray-400 rounded">
                       </div>
                   </div>
                   
                    <button type="submit" class="bg-green-400 py-2 px-4 rounded text-white mt-3">Submit</button>
               </form>
           </div>
           
        </div>
    </div>
</template>
<script>
export default {
    data(){
        return{
          kg:5,
          price:80
        }
    },
    methods: {
        addPrice(e){
           
            this.price++;
             this.kg++;
            e.preventDefault();
            
        },
        reducePrice(e){
           
            this.price--;
             this.kg--;
            e.preventDefault();
            
        }
    },
}
</script>