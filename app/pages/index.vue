
<script setup>
// Data connection goes here tomorrow!
</script>



<template>

  <div class="min-h-screen bg-[#F8FAFC] text-[#000001] font-sans">
    
    <section class="relative h-[500px]  flex items-center bg-gray-400 overflow-hidden">
        
        <img src="../assets/our-hr.png" class="absolute inset-0 w-full h-full object-cover opacity-60" alt=""/>

        <div class="relative max-w-6xl mx-auto px-6 w-full">

            <h1 class="text-white text-5xl font-bold mb-10">Great Careers. 

                <span class=" text-[#1440b8] ">Start here!</span>
            </h1>

            <div class="bg-white p-2 rounded shadow-xl flex flex-col md:flex-row gap-2">
            
                <div class="flex-1 flex items-center px-4 py-2 border-r border-gray-200">
                    <i class="fas fa-search text-gray-400 mr-2"></i>
                    <input type="text" placeholder="Job Title or Keywords" class="w-full outline-none" />
                </div>

                <div class="flex-1 px-4 py-2 border-r border-gray-200 hidden md:block">
                    <select class="w-full outline-none text-gray-500">
                    <option>All Job Functions</option>
                    </select>
                </div>

                <div class="flex-1 px-4 py-2 hidden md:block">
                    <select class="w-full outline-none text-gray-500">
                    <option>All Locations</option>
                    </select>
                </div>

                <button class="bg-[#1440b8] text-white px-10 py-3 rounded font-bold hover:bg-[#7087bb] transition">
                    Find Jobs
                </button>

            </div>

            
        </div>

    </section>

    <section class="py-12 bg-white">
        <div class="max-w-7xl mx-auto px-6">

            <h2 class="text-center text-gray-600 font-bold mb-10 text-xl">Top Employers</h2>

            <div class="flex flex-wrap justify-center gap-3">
            
                <div class="w-[200px] h-[200px] md:w-[120px] md:h-[120px] flex items-center justify-center ">
                    <img src="../assets/our-hr.png" alt="Logo">
                </div>

                <div class="w-[100px] h-[100px] md:w-[120px] md:h-[120px] border border-gray-100 shadow-sm flex items-center justify-center p-2 hover:shadow-md transition bg-white">
                    <img src="" class="max-h-full max-w-full object-contain" alt="Logo">
                </div>

                

            </div>
        </div>
    </section>


    
        


    

    <section class="max-w-6xl mx-auto px-6 py-20">
        <div class="bg-[#1440b8] rounded-2xl p-12 text-center text-white">
            
            <h2 class="text-3xl font-bold mb-4">Are you hiring?</h2>
            
            <p class="text-blue-100 mb-8 max-w-md mx-auto">Post your job opening today and find the best talent for your team.</p>

            <div class="flex flex-col sm:flex-row justify-center gap-4">
            
                <a href="#" class="bg-white text-[#1440b8] hover:bg-[#7087bb] hover:text-white px-10 py-4 rounded-lg font-bold transition duration-300">Post a Job</a>

                <a href="#" class="border border-white text-white hover:bg-white/10 px-10 py-4 rounded-lg font-bold transition duration-300">Learn More</a>

            </div>
        </div>
    </section>
  </div>
</template>

