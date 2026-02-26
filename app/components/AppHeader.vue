<template>
    <header class="bg-slate-50 shadow-xl  items-center justify-between">
        <div class="flex items-center justify-between w-full p-7 pt-0 pb-0">
            <img src="/images/logo1.png" alt="Logo" class=" w-40">
            <div class="flex items-center space-x-4">
                <button class="bg-[rgb(20,64,184)] hover:bg-slate-300 text-gray-700 font-semibold py-2 px-4 rounded">
                    <h1 class="text-white text-1xl hover:text-[#000001] font-semibold">Sign Up</h1>
                    </button>
                    <button class=" border border-gray-300 bg-gray-200 hover:bg-slate-300 text-gray-700 font-semibold py-2 px-4 rounded">
                    <h1 class="text-gray-700 text-1xl hover:text-[#000001] font-semibold">LogIn</h1>
                </button>
            </div>
            
         </div>
         <div class="flex items-center justify-center w-full p-4 pt-0 pb-0">
             <nav class="flex space-x-10 pb-1 ">
                <a href="#" class="relative text-xl group">
                  Home
                  <span class="absolute left-0 -bottom-1 w-0 h-0.5 bg-black transition-all duration-300 group-hover:w-full"></span>
                </a>
                <a href="/list-job" class="relative text-xl group">
                  List Jobs
                  <span class="absolute left-0 -bottom-1 w-0 h-0.5 bg-black transition-all duration-300 group-hover:w-full"></span>
                </a>
                <a href="#" class="relative text-xl group">
                  Jobs Alert
                  <span class="absolute left-0 -bottom-1 w-0 h-0.5 bg-black transition-all duration-300 group-hover:w-full"></span>
                </a>
                <a href="#" class="relative text-xl group">
                  Recommended Jobs
                  <span class="absolute left-0 -bottom-1 w-0 h-0.5 bg-black transition-all duration-300 group-hover:w-full"></span>
                </a>
                <a href="/company" class="relative text-xl group">
                  All Companies
                  <span class="absolute left-0 -bottom-1 w-0 h-0.5 bg-black transition-all duration-300 group-hover:w-full"></span>
                </a>
            
                <a href="#" class="relative text-xl group">
                  Dashboard
                  <span class="absolute left-0 -bottom-1 w-0 h-0.5 bg-black transition-all duration-300 group-hover:w-full"></span>
                </a>
            
            </nav>
         </div>

    </header>

</template>