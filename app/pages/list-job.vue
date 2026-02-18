<template>
  <div class="bg-[#F8FAFC] min-h-screen font-sans antialiased text-[#000001]">
    
    <div class="bg-white border-b border-gray-100 pt-20 pb-24">

        <div class="max-w-6xl mx-auto px-6">
        
            <div class="max-w-2xl">
            
                <h1 class="text-5xl font-black leading-tight mb-4">Find the perfect <br/> 
                    <span class="text-[#1440b8]">job for you.</span>
                </h1>
                
                <p class="text-gray-400 text-lg mb-10">Search and find your dream job with ease.</p>
            </div>
            
            <div class="bg-white p-3 rounded-3xl lg:rounded-full shadow-2xl shadow-blue-900/10 flex flex-col lg:flex-row gap-3 border border-gray-100">
            
                <div class="flex-1 flex items-center px-6 gap-3 border-r-0 lg:border-r border-gray-100">
                    
                    <Icon name="fa6-solid:magnifying-glass" class="text-gray-300 text-xl" />
                    <input type="text" placeholder="Job title or keywords" class="w-full py-4 outline-none text-base bg-transparent" />
                </div>

                <div class="flex-1 flex items-center px-6 gap-3">
                    
                    <Icon name="fa6-solid:location-dot" class="text-gray-300 text-xl" />
                    <input type="text" placeholder="Location" class="w-full py-4 outline-none text-base bg-transparent" />
                </div>
                
                <a href="#">  

                    <button class="bg-[#1440b8] hover:bg-[#7087bb] text-white px-12 py-4 rounded-2xl lg:rounded-full font-bold text-lg transition-all active:scale-95 shadow-lg shadow-blue-900/20">
                    Search</button>
                </a>

            </div>

        </div>

    </div>

    <section class="max-w-6xl mx-auto px-6 py-20">
       
        <div class="mb-12">
            
            <h2 class="text-3xl font-black text-[#000001]">Latest Job Listing</h2>
            <div class="h-1.5 w-12 bg-[#1440b8] mt-2 rounded-full"></div>
        </div>

        <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
                
            <div class="bg-white p-8 rounded-[2.5rem] border hover:shadow-xl transition group">
                
                <div class="flex justify-between items-start mb-6">
                    
                    <div class="w-14 h-14 bg-[#F8FAFC] rounded-2xl flex items-center justify-center border group-hover:border-[#1440b8]">
                        <Icon name="fa6-solid:building" class="text-2xl text-gray-300 group-hover:text-[#1440b8]" />
                    </div>
                    <span class="text-[10px] font-bold text-green-600 bg-green-50 px-3 py-1 rounded-lg">Verified</span>
                        
                </div>

                <h3 class="text-xl font-bold mb-1 group-hover:text-[#1440b8]">UI/UX Designer</h3>
                <p class="text-gray-400 text-sm mb-6 flex items-center gap-2">
                    <Icon name="fa6-solid:location-dot" /> Google Inc.  California
                    <span class="text-[#1440b8] font-bold">$2k - $3k</span>
                </p>

                <div class="flex gap-3 mb-8">
                    <span class="bg-gray-50 text-gray-500 px-3 py-1 rounded-lg text-xs font-bold">Full Time</span>
                    <span class="bg-blue-50 text-[#1440b8] px-3 py-1 rounded-lg text-xs font-black">$ Salary</span>
                </div>

                <a href="#" class="block w-full py-4 bg-[#1440b8] hover:bg-[#7087bb] text-white text-center font-bold rounded-2xl transition">
                    Apply Now
                </a>
                
            </div>
        </div>

    </section>

    

  </div>
</template>