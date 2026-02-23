<template>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/7.0.1/css/all.min.css">
  
  <section class="w-full h-90 url flex bg-[url('https://www.jobnet.com.kh/image/2UtsomdMLD_BCyJzUqHs5u2jWcoM2DXQ7-XjJbIjVfm44rNZdVdadk_lXpeww5Gyn_r2vzQUr80Uh3fbp1R5ydxXG-UFzngrOqOSl7tZw6nOMWmh704vui_tal-CZb2g8W5wW8cvVOiUdqiy20kGHO8dLdnHkq7n')] items-center justify-center">
  </section>

  <div class="max-w-6xl flex justify-center left-45 px-6 absolute -mt-30">
    <div class="flex items-center gap-6">
      <div class="w-36 h-36 bg-white rounded-3xl shadow-xl flex items-center justify-center">
        <img src="https://www.chipmongbank.com/fb-og-image.jpg" class="w-39 h-30 object-contain" alt="Chip Mong Bank" />
      </div>
      <div class="text-white">
        <div class="flex items-center gap-3">
          <h1 class="text-2xl font-bold">Chip Mong Bank</h1>
          <span class="bg-yellow-400 text-black text-xs px-2 py-1 rounded-md font-semibold">Premium</span>
        </div>
        <p class="text-sm text-slate-200 mt-3 ">At Chip Mong Commercial Bank, we strive to be the most trusted bank.</p>
      </div>
    </div>
  </div>

  <div class="w-full m-auto bg-gray-200">
    <div class="max-w-6xl mx-auto ml-88 px-6">
      <ul class="flex items-center gap-10 text-slate-600 font-medium">
        <li @click="activeTab = 'about'" 
            :class="['py-4 cursor-pointer', activeTab === 'about' ? 'border-b-2 border-blue-600 text-blue-600' : 'hover:text-blue-600']">
          About
        </li>

        <li @click="activeTab = 'jobs'" 
            :class="['py-4 cursor-pointer', activeTab === 'jobs' ? 'border-b-2 border-blue-600 text-blue-600' : 'hover:text-blue-600']">
          Jobs
        </li>

        <li @click="activeTab = 'gallery'" 
            :class="['py-4 cursor-pointer', activeTab === 'gallery' ? 'border-b-2 border-blue-600 text-blue-600' : 'hover:text-blue-600']">
          Gallery
        </li>

        <li class="ml-auto absolute left-157 flex gap-4">
          <a href="#" class="w-9 h-9 bg-blue-600 text-white rounded-full flex items-center justify-center"><i class="fa-brands fa-facebook"></i></a>
          <a href="#" class="w-9 h-9 bg-red-600 text-white rounded-full flex items-center justify-center"><i class="fa-brands fa-youtube"></i></a>
        </li>
      </ul>
    </div>
  </div>

  <div class="py-8">
    
    <section v-if="activeTab === 'jobs'">
      
    </section>

    <section v-if="activeTab === 'gallery'" id="media" class="flex w-full max-w-6xl m-auto bg-white">
      <div class="container mx-auto px-4">
        <div class="grid grid-cols-1 gap-4 md:grid-cols-3">
          <div class="md:col-span-2 md:row-span-2">
            <img src="https://www.jobnet.com.kh/image/2UtsomdMLD_BCyJzUqHs5u2jWcoM2DXQ4VL5LukdYAC30zgIMyHW5_TzNwO-lr78AyFYP4MtdmcWmkz8rpIxVzpnQR-KovbFS7_MfsuPnRvatC62X3BAoQ==" class="w-full h-full object-cover rounded-lg" />
          </div>
          <div class="grid grid-cols-2 gap-4 md:grid-cols-1">
            <img src="https://www.jobnet.com.kh/image/2UtsomdMLD_BCyJzUqHs5u2jWcoM2DXQ4VL5LukdYACaxH_CXNHiRGQVS-pWhl509Y2Bc4nx7g0kPFDbAjFG7AxTH-w_cVJEtyzYQk6wL3qIy9_-EeonQw==" class="w-full h-57 object-cover rounded-lg" />
            <img src="https://www.jobnet.com.kh/image/2UtsomdMLD_BCyJzUqHs5u2jWcoM2DXQ4VL5LukdYADDReOaWkclPrBWcEfDrajmRZKVoESebWn4YUA0TbczODyD71PdRRsWxWaDKWcltIlrFkRQcygHig==" class="w-full h-57 object-cover rounded-lg" />
          </div>
        </div>
      </div>
    </section>

    <section v-if="activeTab === 'about'">
     <div class="max-w-6xl mx-auto p-4 font-sans">
  <div class="bg-white border border-gray-200 rounded-sm shadow-sm overflow-hidden">
    
    <div class="p-6">
      <h2 class="text-xl font-bold text-gray-800">Recent job openings</h2>
    </div>

    <div class="grid grid-cols-1 md:grid-cols-3 border-t border-gray-100">
      
      <a href="#" class="group p-6 border-b md:border-b-0 md:border-r border-gray-100 hover:bg-gray-50 transition-colors">
        <h3 class="text-[15px] font-medium text-blue-700 mb-1 group-hover:underline">បុគ្គលិកហាត់ការ ផ្នែកលក់</h3>
        <p class="text-xs text-gray-700 mb-4">Chip Mong Bank</p>
        
        <div class="space-y-2 text-[11px] text-gray-600">
          <div class="flex items-center gap-2">
            <svg class="w-3 h-3 transform rotate-45" fill="currentColor" viewBox="0 0 24 24"><path d="M21 3L3 10.53v.98l6.84 2.65L12.48 21h.98L21 3z"/></svg>
            <span>Svay Rieng</span>
          </div>
          <div class="flex items-center gap-2">
            <svg class="w-3 h-3" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path d="M3 7v10a2 2 0 002 2h14a2 2 0 002-2V9a2 2 0 00-2-2h-6l-2-2H5a2 2 0 00-2 2z"/></svg>
            <span>Sales, Business Development</span>
          </div>
        </div>
      </a>

      <a href="#" class="group p-6 border-b md:border-b-0 md:border-r border-gray-100 hover:bg-gray-50 transition-colors">
        <h3 class="text-[15px] font-medium text-blue-700 mb-1 group-hover:underline">បុគ្គលិកហាត់ការ ផ្នែកលក់</h3>
        <p class="text-xs text-gray-700 mb-4">Chip Mong Bank</p>
        
        <div class="space-y-2 text-[11px] text-gray-600">
          <div class="flex items-center gap-2">
            <svg class="w-3 h-3 transform rotate-45" fill="currentColor" viewBox="0 0 24 24"><path d="M21 3L3 10.53v.98l6.84 2.65L12.48 21h.98L21 3z"/></svg>
            <span>Preah Sihanouk</span>
          </div>
          <div class="flex items-center gap-2">
            <svg class="w-3 h-3" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path d="M3 7v10a2 2 0 002 2h14a2 2 0 002-2V9a2 2 0 00-2-2h-6l-2-2H5a2 2 0 00-2 2z"/></svg>
            <span>Sales, Business Development</span>
          </div>
        </div>
      </a>

      <a href="#" class="group p-6 hover:bg-gray-50 transition-colors">
        <h3 class="text-[15px] font-medium text-blue-700 mb-1 group-hover:underline">បុគ្គលិកហាត់ការ ផ្នែកលក់</h3>
        <p class="text-xs text-gray-700 mb-4">Chip Mong Bank</p>
        
        <div class="space-y-2 text-[11px] text-gray-600">
          <div class="flex items-center gap-2">
            <svg class="w-3 h-3 transform rotate-45" fill="currentColor" viewBox="0 0 24 24"><path d="M21 3L3 10.53v.98l6.84 2.65L12.48 21h.98L21 3z"/></svg>
            <span>Kandal</span>
          </div>
          <div class="flex items-center gap-2">
            <svg class="w-3 h-3" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path d="M3 7v10a2 2 0 002 2h14a2 2 0 002-2V9a2 2 0 00-2-2h-6l-2-2H5a2 2 0 00-2 2z"/></svg>
            <span>Sales, Business Development</span>
          </div>
        </div>
      </a>
    </div>

    <div class="border-t border-gray-100 p-3 text-center">
      <a href="#" class="text-sm font-bold text-blue-800 hover:text-blue-600 transition-colors">
        See All Jobs
      </a>
    </div>
  </div>
</div>
</section>



<section id="media" class="flex w-290 m-auto bg-white py-8">
  <div class="container mx-auto px-4">
    <div>
      <div class="mb-4 text-xl font-bold md:hidden">Gallery</div>

      <div class="grid grid-cols-1 gap-4 md:grid-cols-3">
        
        <div class="md:col-span-2 md:row-span-2">
          <div class="group relative overflow-hidden rounded-lg">
            <a href="https://www.jobnet.com.kh/image/..." class="block">
              <img 
                src="https://www.jobnet.com.kh/image/2UtsomdMLD_BCyJzUqHs5u2jWcoM2DXQ4VL5LukdYAC30zgIMyHW5_TzNwO-lr78AyFYP4MtdmcWmkz8rpIxVzpnQR-KovbFS7_MfsuPnRvatC62X3BAoQ==" 
                alt="Featured" 
                class="h-117 w-full object-cover transition-transform duration-300 group-hover:scale-105"
                style="aspect-ratio: 570 / 400;"
              />
            </a>
          </div>
        </div>

        <div class="grid grid-cols-2 gap-4 md:grid-cols-1">
          
          <div class="overflow-hidden rounded-lg">
            <a href="#" class="block">
              <img src="https://www.jobnet.com.kh/image/2UtsomdMLD_BCyJzUqHs5u2jWcoM2DXQ4VL5LukdYACaxH_CXNHiRGQVS-pWhl509Y2Bc4nx7g0kPFDbAjFG7AxTH-w_cVJEtyzYQk6wL3qIy9_-EeonQw==" 
                   class="h-full w-full object-cover" alt="Gallery small" />
            </a>
          </div>

          <div class=" relative overflow-hidden rounded-lg">
            <a href="#" class="block">
              <img src="https://www.jobnet.com.kh/image/2UtsomdMLD_BCyJzUqHs5u2jWcoM2DXQ4VL5LukdYADDReOaWkclPrBWcEfDrajmRZKVoESebWn4YUA0TbczODyD71PdRRsWxWaDKWcltIlrFkRQcygHig==" 
                   class="h-full w-full object-cover" alt="Gallery small" />
            </a>
            <div class="absolute bottom-0 left-0 right-0 cursor-pointer rounded-lg md:block hidden">
            <a href="#career-video" class="flex h-57   items-center justify-center bg-black/50 text-white hover:bg-black/60 transition">
              <span class="font-semibold uppercase tracking-wider">View More</span>
            </a>
          </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>


<section class="">
  <div class="container mx-auto px-4 max-w-6xl">
    <div class=" rounded-xl shadow-sm border border-gray-100 overflow-hidden">
      
      <div class="p-6 md:p-10">
        
        <h2 class="text-2xl md:text-3xl text-gray-800 mb-8 border-b pb-4">
          About Chip Mong Bank
        </h2>

        <div class="grid grid-cols-1 md:grid-cols-2 gap-8 mb-10">
          
          <div class="space-y-4">
            <div class="flex items-center gap-3 text-blue-600">
              <div class="flex items-center justify-center w-4 h-4 bg-gray-300 p-4 rounded-full">
                <i class="text-[14px] text-black fa-regular fa-user"></i>
              </div>
              <h3 class=" text-lg text-gray-700 uppercase tracking-wide">Employer Details</h3>
            </div>
            
            <ul class="space-y-3 bg-gray-50 p-4 rounded-lg">
              <li class="flex justify-between border-b border-gray-200 pb-2">
                <span class="text-gray-500 ">Type:</span>
                <span class="text-gray-800  text-right">Direct Employer</span>
              </li>
              <li class="flex justify-between border-b border-gray-200 pb-2">
                <span class="text-gray-500 ">Industry:</span>
                <span class="text-gray-800 text-right text-sm md:text-base">Banking/ Insurance/ Microfinance</span>
              </li>
              <li class="flex justify-between">
                <span class="text-gray-500 ">No. Employees:</span>
                <span class="text-gray-800 text-right">1001 to 5000</span>
              </li>
            </ul>
          </div>

          <div class="space-y-4">
            <div class="flex items-center gap-3 text-blue-600">
              <div class="flex items-center justify-center w-8 h-8 bg-gray-300 rounded-full">
                <i class="fa-solid fa-location-arrow text-black"></i>
              </div>
              <h3 class="text-lg text-gray-700 uppercase tracking-wide">Address</h3>
            </div>
            <div class=" p-4 rounded-lg h-full">
              <p class="text-gray-600 leading-relaxed">
                No 174 (3rd & 4th floor), Czech Republic Blvd. Corner Street No 164, Sangkat Veal Vong, Khan Prampir Meakkara, Phnom Penh, Cambodia
              </p>
            </div>
          </div>
        </div>

        <hr class="mb-10 border-gray-100" />

        <div class="space-y-10">
          
          <div class="group">
            <div class="flex items-center gap-3 text-blue-600 mb-4">
              <div class="flex items-center justify-center w-8 h-8 bg-blue-50 rounded-full  ">
                <i class="fa-solid fa-brain text-black"></i>
              </div>
              <h3 class=" text-lg text-gray-700 uppercase tracking-wide">Company Vision and Mission</h3>
            </div>
            <p class="text-gray-600 leading-relaxed text-lg pl-11">
              At Chip Mong Commercial Bank, we strive to be the most trusted bank in the country, offering innovative financial solutions to our retail and business customers. With a strong commitment to excellence, collaboration, integrity, and making a difference, we aim to help our customers grow financially.
            </p>
          </div>

          <div class="group">
            <div class="flex items-center gap-3 text-blue-600 mb-4">
              <div class="flex items-center justify-center w-8 h-8 bg-blue-50 rounded-full">
                <i class="fa-regular fa-folder text-black"></i>
              </div>
              <h3 class="text-lg text-gray-700 uppercase tracking-wide">What we do</h3>
            </div>
            <p class="text-gray-600  text-lg pl-11">
              We warmly welcome you into our big family to share in our vision to establish one of the most admired and respected digital-centric banks in Cambodia. We want you to feel proud about the opportunities with us, because we can assure you that you will always be well taken care of, as we boost your personal and professional development. Like us, you will love our fashionable office environment, share in the same joy of working and be passionate about innovation as we grow the bank.
            </p>
          </div>

        </div>

        <div class="mt-12 text-center md:text-left md:pl-11">
            <button class="bg-[#1440b8] text-white px-8 py-3 rounded-lg shadow-lg hover:bg-blue-700 transition transform ">
                Join Us Now!
            </button>
              <div class="relative bottom-8 left-1/2 transform -translate-x-1/2">
            <h3 class="text-slate-600 ml-103 max-md mx-auto">Follow our social media</h3>
            <div class="flex h-10 w-full justify-center mt-2">
                <i class="fa-brands fa-linkedin h-6 w-10 text-slate-600 hover:text-indigo-600 transition-colors mx-2"></i>
                <i class="fa-brands fa-twitter h-6 w-10 text-slate-600 hover:text-indigo-600 transition-colors mx-2"></i>
                <i class="fa-brands fa-facebook h-6 w-10 text-slate-600 hover:text-indigo-600 transition-colors mx-2"></i>
                <i class="fa-brands fa-instagram h-6 w-10 text-slate-600 hover:text-indigo-600 transition-colors mx-2"></i>
            </div>
        </div>
        </div>

      </div>
    </div>
  </div>
    </section>

  </div>
</template>

<script setup>
import { ref } from 'vue'
const activeTab = ref('about')
</script>