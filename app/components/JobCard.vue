<script setup>

const props = defineProps({
  company: String,
  title: String,
  salary: String,
  date: String
})

</script>

<template>
  
  <div class="bg-white rounded-[40px] border border-gray-100 hover:shadow-xl transition-all">
    
    <div class="bg-blue-100 p-8 rounded-[40px]">
      
        <div class="flex justify-between mb-4">
            <span class="py-1 rounded-lg text-[10px] font-bold">{{ date }}</span>
            <Icon name="mdi:twitter" class="text-blue-600 text-2xl" />
         </div>
      
        <p class="text-xs font-bold text-blue-800 uppercase">{{ company }}</p>
        <h3 class="text-xl font-bold mt-1">{{ title }}</h3>
        
        <div class="flex gap-2 mt-4 flex-wrap">
            <span class="bg-blue-200/50 px-2 py-1 rounded text-[10px] font-bold">Full time</span>
            <span class="bg-blue-200/50 px-2 py-1 rounded text-[10px] font-bold">Part time</span>
        
        </div>
    </div>

    <div class="flex justify-between items-center p-4 mt-2">
      
        <p class="font-black text-lg">${{ salary }}/month</p>
      
        <button class="bg-[#1440b8] text-white px-8 py-3 rounded-full font-bold text-sm">Details</button>
    </div>
  
  </div>
</template>