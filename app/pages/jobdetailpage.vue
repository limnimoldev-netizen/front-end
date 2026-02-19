<template>
    <div class="pl-10 pr-10">
        <h1 class="text-4xl font-bold  mt-10">
            Web Engineer- Frontend UI Developer
            
        </h1>
            <div class="flex gap-10">
                <p class=" text-xl mt-5 font-normal mt-2 text-gray-500 flex items-center gap-2" >
                    <Icon name="mdi:location-outline" class="text-gray-500 text-3xl mb-1.5 " />
                    Stoemg Mean Chey 
                </p>
                <p class=" text-xl mt-5 font-normal text-gray-500 mt-2 flex items-center gap-2" >
                    <Icon name="mdi:briefcase-outline" class="text-gray-500 text-3xl mb-1.5 " />
                    Full time 
                </p>
            </div>
            <div    class="mt-10 flex space-between gap-20">
                <div class="w-2/3">
                    <h1 class="text-3xl font-bold mt-10 ">
                         What We do
                    </h1 class=" border-b ">
                        <p class="text-xl w-230 mt-5 font-normal text-gray-500 mt-2 border-b-2 border-gray-300 pb-2 " >
                           A Web Engineer – Frontend UI Developer is responsible 
                           for designing and devborder-gray-300 pb-5eloping the user interface  of web 
                           applications to ensure a smooth, responsive, and engaging
                            user experience. In this role, we build  interactive web 
                            pages using technologies such as HTML, CSS, JavaScript, 
                            and modern frameworks like  Vue.js or React. We transform UI/UX designs 
                            into functional websites, integrate APIs to display dynamic data, and ensure 
                            compatibility across different devices and browsers. We also optimize performance, 
                            maintain clean  and reusable code, fix bugs, and collaborate closely with backend
                             developers and designers to deliver high-quality  digital products that meet business 
                             and user needs. 
                        </p>
                    
                    <h1 class="text-3xl font-bold mt-15 ">
                         Job
                        Tasks
                    </h1>
                        <p class="text-xl w-230 mt-5 font-normal text-gray-500 mt-2 border-b-2 border-gray-300 pb-5" >
                            - Collaborate with designers and backend developers to create responsive and user-friendly web applications.<br>
                            - Develop and maintain the frontend architecture of web applications using modern frameworks like Vue.js or React.<br>
                            - Write clean, efficient, and well-documented code to implement UI components and features.<br>
                            - Optimize web applications for maximum speed and scalability.<br>
                            - Ensure cross-browser compatibility and responsiveness across various devices.<br>
                            - Integrate APIs to fetch and display dynamic data on the frontend.<br>
                            - Conduct code reviews and provide constructive feedback to team members.<br>
                            - Stay updated with the latest industry trends and best practices in frontend development.<br>
                            - Troubleshoot and debug issues to ensure a seamless user experience.<br>
                            - Collaborate with backend developers to ensure smooth integration of frontend and backend functionalities.
                        </p>

                        <button @click="toggleLetter" type="button" class="  font-semibold py-2  flex rounded mt-5">
                            <h1 class="text-3xl font-bold ">Requirements </h1>
                           <h1 class="text-3xl font-bold ">
                                
                             <Icon name="heroicons:chevron-down" class="w-5 h-5 mt-2  ml-2 transition-transform duration-300"
                              :class="showLetter ? 'rotate-180 ' : ''" />
                           </h1>
                            
                        </button>
                        <div v-if="showLetter" class="mt-4">
                    
                            <p class="text-xl w-230 mt-5 font-normal text-gray-500 mt-2 border-b-2 border-gray-300 pb-5" >
                                - Proven experience as a Frontend UI Developer or similar role.<br>
                                - Proficiency in HTML, CSS, JavaScript, and modern frontend frameworks like Vue.js or React.<br>
                                - Strong understanding of responsive design principles and cross-browser compatibility.<br>
                                - Experience with version control systems (e.g., Git) and collaborative development workflows.<br>
                                - Knowledge of UI/UX design principles and ability to translate designs into functional web interfaces.<br>
                                - Familiarity with RESTful APIs and integration of frontend applications with backend services.<br>
                                - Excellent problem-solving skills and attention to detail.<br>
                                - Strong communication and teamwork abilities to collaborate effectively with designers, backend developers, and other stakeholders.<br>
                                - A portfolio showcasing previous frontend projects is a plus.
                            </p>
                        </div>

                        <button @click="toggleLetter2" type="button" class="  font-semibold py-2  flex rounded mt-5">
                            <h1 class="text-3xl font-bold ">Benefits </h1>
                           <h1 class="text-3xl font-bold ">
                                
                             <Icon name="heroicons:chevron-down" class="w-5 h-5 mt-2  ml-2 transition-transform duration-300"
                              :class="showLetter2 ? 'rotate-180 ' : ''" />
                           </h1>
                            
                        </button>
                        <div v-if="showLetter2" class="mt-4">
                    
                            <p class="text-xl w-230 mt-5 font-normal text-gray-500 mt-2 border-b-2 border-gray-300 pb-5" >
                                - Health insurance coverage<br>
                                - Flexible working hours<br>
                                - Remote work options<br>
                                - Professional development opportunities<br>
                                - Performance-based bonuses<br>
                                - Paid time off and holidays<br>
                                - Employee stock options (if applicable)<br>
                                - A portfolio showcasing previous frontend projects is a plus.
                                
                            </p>
                        </div>

                        

                </div>
                <div class="mt-14 shadow-md bg-white border h-64 border-gray-200 rounded-lg w-full  text-center">
                    <h1 class="text-xl mt-5     font-bold text-black-500">
                        Interested in this job?
                    </h1>
                    <div class="p-4 flex bg-gray-100 gap-3">
                        <img src="/images/cto.png" alt="CTO Image" class="w-20 h-20 shadow-lg border-gray-300  rounded-full">
                        <div class="text-left">
                            <h1 class="text-1xl text-gray-500">
                                Contact person
                            </h1>
                            <h1 class="text-2xl font-bold">
                                Mr.Rock
                            </h1>
                            <h1>
                                CTO
                            </h1>
                        </div>
                    </div>
                  <div class="max-w-md mx-auto bg-white p-6 rounded-lg shadow-md">
    
                  
                    <div class="grid grid-cols-2 gap-4">
                      <div>
                        <label class="text-sm text-gray-500">First Name</label>
                        <input
                          type="text"border-gray-300 pb-5
                          class="w-full border-b border-gray-300 focus:outline-none focus:border-[rgb(20,64,184)] py-2"
                        />
                      </div>
                    
                      <div>
                        <label class="text-sm text-gray-500">Last Name</label>
                        <input
                          type="text"
                          class="w-full border-b border-gray-300 focus:outline-none focus:border-[rgb(20,64,184)]  py-2"
                        />
                      </div>
                    </div>
                
                  
                    <div class="mt-6">
                      <label class="text-sm text-gray-500">Email</label>
                      <input
                        type="email"
                        class="w-full border-b border-gray-300 focus:outline-none focus:border-[rgb(20,64,184)] py-2"
                      />
                    </div>
                
                  
                    <div class="mt-6">
                      <label class="text-sm text-gray-500">Phone Number</label>
                      <input
                        type="text"
                        class="w-full border-b border-gray-300 focus:outline-none focus:border-[rgb(20,64,184)] py-2"
                      />
                    </div>
                
                    border-gray-300 pb-5
                    <div class="mt-6">
                      <p class="text-sm text-gray-600">
                        Documents:
                        <span class="text-gray-400 text-xs">.doc, .docx, .pdf, .rtf, .txt</span>
                      </p>
                    
                    
                      <label
                        class="flex items-center justify-center gap-2 bg-gray-100 text-green-700 py-3 rounded-lg mt-3 cursor-pointer hover:bg-slate-300 transition"
                      >
                        📎 <span>CV</span>
                        <input type="file" class="hidden" />
                      </label>border-gray-300 pb-5
                    
                      
                      <label
                        class="flex items-center justify-center gap-2 bg-gray-100 text-green-700 py-3 rounded-lg mt-3 cursor-pointer hover:bg-slate-300 transition"
                      >
                        📎 <span>COVER LETTER <span class="text-gray-400">(optional)</span></span>
                        <input type="file" class="hidden" />
                      </label>

                      <button type="submit" class="w-full bg-[rgb(20,64,184)] text-white py-3 rounded-lg mt-6 hover:text-[#000001] hover:bg-slate-300 transition">
                       APPLY NOW
                      </button>
                    </div>
                
                   
                   
                    </div>
                          
                </div>
                
            </div>

    </div>
</template>
<script setup>

import { ref } from 'vue';

const showLetter = ref(false);

const toggleLetter = () => {
  showLetter.value = !showLetter.value;
};




const showLetter2 = ref(false);

const toggleLetter2 = () => {
  showLetter2.value = !showLetter2.value;
};
</script>
