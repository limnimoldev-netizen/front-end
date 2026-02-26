<script setup>

import JobCard from '@/components/JobCard.vue';

const categories = [
  { name: 'Development',
   jobs: 16, 
   icon: 'mdi:code-tags' },

  { name: 'Marketing',
   jobs: 8, 
   icon: 'mdi:bullhorn-outline' },

  { name: 'Design', 
  jobs: 13,
   icon: 'mdi:palette-outline' },

  { name: 'Service',
   jobs: 8, 
   icon: 'mdi:account-heart-outline' }
   
]

</script>

<template>

   
    <section class="relative w-full min-h-[550px] flex items-center justify-center text-center px-4 overflow-hidden">
            
        <div class="absolute inset-0">
            
            <img src="../assets/our-hr.png" alt="" class="w-full h-full object-cover" />
            <div class="absolute inset-0 bg-white/40"></div>
        </div>

        <div class="relative z-10 flex flex-col items-center">
                
            <h1 class="text-[#1440b8] text-5xl md:text-6xl font-black mb-6 leading-tight max-w-3xl">
                Modernizing the Job <br> Search Experience</h1>
               
            <p class="text-slate-900 mb-10 max-w-md mx-auto font-medium">
                Search and find your dream job easier than ever. Simply browse and find a job if you need it.</p>
                
            <div class="bg-white p-2 rounded-full shadow-2xl flex items-center w-full max-w-xl border border-gray-100">

                <input type="text" placeholder="Search for a Job..." class="flex-1 px-6 outline-none text-slate-800 bg-transparent"/>
                <button class="bg-[#1440b8] text-white px-8 py-3 rounded-full font-bold hover:bg-blue-700 transition active:scale-95">
                    Search</button>
                    
            </div>
        
        </div>

    </section>

    <section class="grid grid-cols-1 md:grid-cols-3 gap-8 py-16 max-w-6xl mx-auto text-center px-6">
            
        <div>
            
            <h2 class="text-4xl font-black text-slate-900">91%</h2>
                
                <p class="font-bold text-blue-600 mt-1">Skills Aligned</p>
                <p class="text-gray-400 text-sm mt-2">Trusted data from our top recruitment partners.</p>
            </div>

            <div>
                
                <h2 class="text-4xl font-black text-slate-900">90%</h2>
                <p class="font-bold text-blue-600 mt-1">Fast and Efficient</p>
                <p class="text-gray-400 text-sm mt-2">Trusted data from our top recruitment partners.</p>
            </div>

            <div>
               
                <h2 class="text-4xl font-black text-slate-900">89%</h2>
                <p class="font-bold text-blue-600 mt-1">Wide Range</p>
                
                <p class="text-gray-400 text-sm mt-2">Trusted data from our top recruitment partners.</p> 
            </div>

    </section>

        
    <section class="max-w-6xl mx-auto py-10 px-6">
            
        <div class="text-center mb-10">
            
            <h2 class="text-3xl font-black text-[#1440b8]">Popular Categories</h2>
        </div>

        <div class="grid grid-cols-1 lg:grid-cols-4 gap-6">
            
            <div v-for="cat in categories" :key="cat.name" class="bg-gray-50 p-8 rounded-3xl border border-gray-100 hover:bg-blue-50 transition">
                
                <div class="w-14 h-14 bg-white rounded-2xl flex items-center justify-center mb-4">
                    <Icon :name="cat.icon" class="text-blue-500 text-3xl" />
                </div>
                
                <h3 class="font-bold text-xl">{{ cat.name }}</h3>
                <p class="text-gray-500 text-sm">{{ cat.jobs }} jobs available</p>
            </div>
        
        </div>
                    
    </section>


    <section class="max-w-6xl mx-auto py-20 px-6">
      
        <div class="text-center mb-12">
            <h2 class="text-3xl font-black text-[#1440b8]">Recommended Jobs</h2>
            <p class="text-gray-400 mt-2">Trusted by thousands of job seekers worldwide.</p>
        </div>
      
      <div class="grid grid-cols-1 md:grid-cols-3 gap-8 mb-12">
        <JobCard 
          company="Twitter" 
          title="UX Designer" 
          salary="800" 
          date="12 Feb 2024" />
        
          <JobCard 
          company="Facebook" 
          title="Product Manager" 
          salary="1200" 
          date="15 Feb 2024" />
        
          <JobCard 
          company="Google" 
          title="Frontend Developer" 
          salary="1500" 
          date="20 Feb 2024" />
      
        </div>

      <div class="flex justify-center">
       
        <router-link to="/list-job">
          
            <button class="bg-[#1440b8] text-white px-9 py-4 rounded-full font-bold hover:bg-blue-700 transition">View More</button>
        
        </router-link>
      
    </div>

    </section>
 
    <section class="max-w-6xl mx-auto p-6 my-10">

        <div class="text-center mb-10">
               
            <h2 class="text-3xl font-black text-[#1440b8]">She How It Works</h2>             
            <p class="text-gray-400 mt-2">Trusted by thousands of job seekers worldwide.</p>
        </div>
          
        <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
               
            <div class="bg-blue-50 p-8 rounded-xl  relative">
                 
                <span class="text-[#1440b8] text-xs font-bold uppercase">Step 01</span>
                    
                    <h3 class="text-lg font-bold mt-2 mb-3">Register An Account</h3>
                    <p class="text-gray-500 text-sm leading-relaxed">
                        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor. </p>   
            </div>

            <div class="bg-blue-50 p-8 rounded-xl ">
                
                <span class="text-[#1440b8] text-xs font-bold uppercase">Step 02</span>
                <h3 class="text-lg font-bold mt-2 mb-3">Search Your Job</h3>
                <p class="text-gray-500 text-sm leading-relaxed">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor.</p>

            </div>

            <div class="bg-blue-50 p-8 rounded-xl ">
               
                <span class="text-[#1440b8] text-xs font-bold uppercase">Step 03</span>         
               
                <h3 class="text-lg font-bold mt-2 mb-3">Apply For Job</h3>      
                <p class="text-gray-500 text-sm leading-relaxed">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor.</p>
               
            </div>

        </div>

    </section>

        
    <section class="max-w-6xl mx-auto p-6 my-10">
            
        <div class="text-center mb-10">
                
            <h2 class="text-3xl font-black text-[#1440b8]">What Our Customers Say</h2> 
            <p class="text-gray-400 mt-2">Trusted by thousands of job seekers worldwide.</p>
            
        </div>
  
        <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
                
            <div class="bg-blue-50 p-8 rounded-[2rem] border border-blue-100 transition hover:shadow-md">
                    
                <div class="flex items-center gap-4 mb-4">
                        
                    <div class="w-[60px] h-[60px] bg-white border rounded-4xl overflow-hidden shadow-sm">
                            
                        <img src="../assets/pf1.png" alt="User Profile" class="w-full h-full object-cover">
                        
                    </div>
                        
                    <div>   
                        <h4 class="font-bold text-slate-900">Alex Johnson</h4>    
                        <p class="text-xs text-blue-600 font-bold">Product Designer</p>     
                    </div>
                   
                </div>
                    
                <p class="text-gray-600 text-sm leading-relaxed">
                "HireMe made my job search so easy. I found a position at Gojek within a week of signing up! The interface is very friendly and modern.</p>
                    
                <div class="mt-4 flex gap-1 text-yellow-500">
                      
                    <Icon name="mdi:star" class="text-xl" />
                    <Icon name="mdi:star" class="text-xl" />
                    <Icon name="mdi:star" class="text-xl" />
                    <Icon name="mdi:star" class="text-xl" />
                    <Icon name="mdi:star" class="text-xl" />
                    
                </div>
                
                
            </div>

                
            <div class="bg-blue-50 p-8 rounded-[2rem] border border-blue-100 transition hover:shadow-md">
                    
                   
                <div class="flex items-center gap-4 mb-4">
                       
                    <div class="w-[60px] h-[60px] bg-white border rounded-4xl overflow-hidden shadow-sm">
                           
                        <img src="../assets/pf1.png" alt="User Profile" class="w-full h-full object-cover">   
                    </div>
                            
                    <div>
                       
                        <h4 class="font-bold text-slate-900">Sarah Williams</h4>                  
                        <p class="text-xs text-blue-600 font-bold">UX Researcher</p>
                    </div>
                    
            </div>
                    
                <p class="text-gray-600 text-sm leading-relaxed">
                "I love the Recommended Jobs feature. It actually understands my skills and suggests things I'm actually interested in. Highly recommended!"</p>
                        
                <div class="mt-4 flex gap-1 text-yellow-500">
                    <Icon name="mdi:star" class="text-xl" />
                    <Icon name="mdi:star" class="text-xl" />
                    <Icon name="mdi:star" class="text-xl" />
                    <Icon name="mdi:star" class="text-xl" />
                    <Icon name="mdi:star" class="text-xl" />
                </div>  
            </div>
            
        </div>

    </section>


    <section class="max-w-6xl mx-auto px-6 py-20"> 
            
        <div class="text-center mb-12">
               
            <h2 class="text-4xl font-black mt-2">Find Expert Tips and Growth <br>  
                <span class="text-[#1440b8]">Insights on Our Blog</span>
            </h2>
        </div>

        <div class="grid lg:grid-cols-2 gap-12">   
                    
            <div>    
                <div class=" rounded-[30px]  mb-6 overflow-hidden">
                     
                    <img src="../assets/hr-blog2.png" alt="Blog" class="w-full h-full object-cover">   
                </div>

                    
                <h3 class="text-3xl font-black mb-4">How to Spot Recruitment Fraud.</h3>
                    
                    
                <p class="text-gray-500 mb-6 leading-relaxed">
                Recruitment fraud is a crime that involves the creation of fictitious job opportunities using trusted brands...</p>
                       
                <button class="bg-blue-600 text-white px-8 py-3 rounded-full font-bold hover:bg-[#7087bb] transition">Learn More</button>      
            </div>

            <div class="space-y-8">
                    
                <div class="flex gap-6 items-center">
                        
                    <div class="w-32 h-24 bg-gray-200 rounded-2xl flex-shrink-0 overflow-hidden">
                            
                        <img src="../assets/hr-blog1.png" alt="Tip" class="w-full h-full object-cover">    
                    </div>
     
                    <div>
                        <h4 class="font-black text-lg leading-tight mb-2">Video Interview Tips: Before, During, <br>and After</h4>
                            
                    </div>
                </div>

                <div class="flex gap-6 items-center">
                        
                    <div class="w-32 h-24 bg-gray-200 rounded-2xl flex-shrink-0 overflow-hidden">
                        
                        <img src="../assets/hr-blog3.png" alt="Tip" class="w-full h-full object-cover">
                    </div>
                        
                    <div>
                        <h4 class="font-black text-lg leading-tight mb-2">Maximizing Your Job Search Potential with AI Tools</h4>
                        
                    </div>
                </div>

                    
                <div class="flex gap-6 items-center">
                        
                    <div class="w-32 h-24 bg-gray-200 rounded-2xl overflow-hidden">
                            
                        <img src="../assets/hr-blog4.png" alt="Tip" class="w-full h-full object-cover">  
                    </div>
                        
                    <div>  
                        <h4 class="font-black text-lg leading-tight mb-2">Top 5 LinkedIn Tips for Job </h4>
                                  
                    </div>
                    
                </div>
            </div>

            
        </div>

    </section>


    <section class="max-w-6xl mx-auto px-6 pb-20">

        <div class="relative w-full bg-blue-50 rounded-[40px] p-12  overflow-hidden ">
                
            <div class="relative z-10 ">
                
                <h2 class="text-4xl font-black mb-6  text-blue-950">Transforming the Way <br> you Find Jobs</h2>
                <p class="text-blue-700/70 mb-10 font-medium">Stop searching, start discovering. Let the ideal job <br> come to you.</p>

                <div class="bg-white p-1.5 rounded-full flex items-center  max-w-sm border border-blue-100">
                            
                    <input type="email" placeholder="Enter your email" class="flex-1 px-5 outline-none text-sm bg-transparent"/>
                    <button class="bg-blue-600 text-white px-8 py-3 rounded-full font-bold text-sm hover:bg-[#7087bb] ">Subscribe</button>
                            
                </div>
                    
            </div>

            <div class="absolute right-0 bottom-0   ">
                <img src="../assets/hrsub.png" alt="">

            </div>

        </div> 
    </section>


</template>