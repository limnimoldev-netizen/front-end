<script setup>
import { ref, computed } from 'vue';

const allCompanies = ref([
  {
    name: 'ABA BANK',
    industry: 'Information Technology',
    logo: 'https://i.ibb.co/7JRfpS4m/aba-1.jpg',
    bannerImage: 'https://careers.ababank.com/job-posting/ABA-basic-banking-new_24.jpg',
    profileUrl: 'https://www.ababank.com/app/?gad_source=1&gad_campaignid=793541930&gbraid=0AAAAADh3gSPvwFldMg_w8ECAsGSWUQT20&gclid=Cj0KCQiA49XMBhDRARIsAOOKJHZHPGnYnJg6beORQdaHR2Sg98ssPWZ0dlgfYByq_s2POuLwWx3xj7UaAtTGEALw_wcB'
  },

  {
    name: 'ACELEDA BANK',
    industry: 'Information Technology',
    logo: 'https://assets.weforum.org/organization/image/oW42OTEcgNgP2WDuDnO38N1bnVQcAeYm7TnLJlxF0OE.jpg',
    bannerImage: 'https://cambodiainvestmentreview.com/wp-content/uploads/2021/05/Edit-Building-2021-scaled.jpg',
    profileUrl: 'https://www.acledabank.com.kh/kh/eng/'
  },
  {
    name: 'WING BANK',
    industry: 'Information Technology',
    logo: 'https://play-lh.googleusercontent.com/A8bangMCdTPS1Xa9hbuc4pcXxUspKpJhDHWW3QSw3OB-VMtUv6NCnqAd7pUv2C-2OnjJHn0Xmv1cs6c2hFUZMw',
    bannerImage: 'https://cfi.co/wp-content/uploads/2022/12/WC104858-jpg.webp',
    profileUrl: 'https://www.wingbank.com.kh/en/news/a-cambodian-womans-journey-from-a-garment-worker-to-business-leader?gad_source=1&gad_campaignid=23581817479&gbraid=0AAAAAonc9UCI2ZIikUhCc03XzAjwgZ6tH&gclid=Cj0KCQiA49XMBhDRARIsAOOKJHaTcvdj51eE9mZcF4qbqpBzNvina-Y9saRB5l3iNJxpGhCUfka6FEcaAi_VEALw_wcB'
  },
  {
    name: 'ABA BANK',
    industry: 'Information Technology',
    logo: 'https://i.ibb.co/7JRfpS4m/aba-1.jpg',
    bannerImage: 'https://careers.ababank.com/job-posting/ABA-basic-banking-new_24.jpg',
    profileUrl: 'https://www.ababank.com/app/?gad_source=1&gad_campaignid=793541930&gbraid=0AAAAADh3gSPvwFldMg_w8ECAsGSWUQT20&gclid=Cj0KCQiA49XMBhDRARIsAOOKJHZHPGnYnJg6beORQdaHR2Sg98ssPWZ0dlgfYByq_s2POuLwWx3xj7UaAtTGEALw_wcB'
  },
  {
    name: 'ABA BANK',
    industry: 'Information Technology',
    logo: 'https://i.ibb.co/7JRfpS4m/aba-1.jpg',
    bannerImage: 'https://careers.ababank.com/job-posting/ABA-basic-banking-new_24.jpg',
    profileUrl: 'https://www.ababank.com/app/?gad_source=1&gad_campaignid=793541930&gbraid=0AAAAADh3gSPvwFldMg_w8ECAsGSWUQT20&gclid=Cj0KCQiA49XMBhDRARIsAOOKJHZHPGnYnJg6beORQdaHR2Sg98ssPWZ0dlgfYByq_s2POuLwWx3xj7UaAtTGEALw_wcB'
  },
  {
    name: 'ABA BANK',
    industry: 'Information Technology',
    logo: 'https://i.ibb.co/7JRfpS4m/aba-1.jpg',
    bannerImage: 'https://careers.ababank.com/job-posting/ABA-basic-banking-new_24.jpg',
    profileUrl: 'https://www.ababank.com/app/?gad_source=1&gad_campaignid=793541930&gbraid=0AAAAADh3gSPvwFldMg_w8ECAsGSWUQT20&gclid=Cj0KCQiA49XMBhDRARIsAOOKJHZHPGnYnJg6beORQdaHR2Sg98ssPWZ0dlgfYByq_s2POuLwWx3xj7UaAtTGEALw_wcB'
  },
  {
    name: 'ABA BANK',
    industry: 'Information Technology',
    logo: 'https://i.ibb.co/7JRfpS4m/aba-1.jpg',
    bannerImage: 'https://careers.ababank.com/job-posting/ABA-basic-banking-new_24.jpg',
    profileUrl: 'https://www.ababank.com/app/?gad_source=1&gad_campaignid=793541930&gbraid=0AAAAADh3gSPvwFldMg_w8ECAsGSWUQT20&gclid=Cj0KCQiA49XMBhDRARIsAOOKJHZHPGnYnJg6beORQdaHR2Sg98ssPWZ0dlgfYByq_s2POuLwWx3xj7UaAtTGEALw_wcB'
  },
  {
    name: 'ABA BANK',
    industry: 'Information Technology',
    logo: 'https://i.ibb.co/7JRfpS4m/aba-1.jpg',
    bannerImage: 'https://careers.ababank.com/job-posting/ABA-basic-banking-new_24.jpg',
    profileUrl: 'https://www.ababank.com/app/?gad_source=1&gad_campaignid=793541930&gbraid=0AAAAADh3gSPvwFldMg_w8ECAsGSWUQT20&gclid=Cj0KCQiA49XMBhDRARIsAOOKJHZHPGnYnJg6beORQdaHR2Sg98ssPWZ0dlgfYByq_s2POuLwWx3xj7UaAtTGEALw_wcB'
  },
  {
    name: 'ABA BANK',
    industry: 'Information Technology',
    logo: 'https://i.ibb.co/7JRfpS4m/aba-1.jpg',
    bannerImage: 'https://careers.ababank.com/job-posting/ABA-basic-banking-new_24.jpg',
    profileUrl: 'https://www.ababank.com/app/?gad_source=1&gad_campaignid=793541930&gbraid=0AAAAADh3gSPvwFldMg_w8ECAsGSWUQT20&gclid=Cj0KCQiA49XMBhDRARIsAOOKJHZHPGnYnJg6beORQdaHR2Sg98ssPWZ0dlgfYByq_s2POuLwWx3xj7UaAtTGEALw_wcB'
  },
  // Add more company objects here to test the "Load More" button
]);

// Load More Logic
const displayLimit = ref(6); // Show 3 at a time
const loadMore = () => {
  displayLimit.value += 3;
};

const visibleCompanies = computed(() => {
  return allCompanies.value.slice(0, displayLimit.value);
});

const hasMore = computed(() => {
  return displayLimit.value < allCompanies.value.length;
});
</script>

<template>
  <div class="min-h-screen bg-[#F8FAFC] text-[#000001] font-sans">
    <section class="bg-[#1440b8] py-16 px-6 text-white">
    <div class="max-w-7xl mx-auto grid grid-cols-1 md:grid-cols-2 items-center gap-12">
      
      <div class="text-left">
        <h1 class="text-5xl font-extrabold mb-6 tracking-tight leading-tight">
          DISCOVER YOUR FUTURE <br> 
          <span class="text-[#000001]">GREAT COMPANY</span>
        </h1>
        <p class="text-blue-100 text-lg">
          Connecting talented professionals with the world's most innovative organizations.
        </p>
        <button class="bg-[#32CD32] text-white px-8 mt-4 py-3 rounded-lg font-bold hover:bg-emerald-600 transition-all">
          Get Started
        </button>
      </div>

      <div class="hidden md:block">
        <img 
          src="https://img.freepik.com/free-vector/job-interview-conversation_74855-7566.jpg" 
          alt="Business Team" 
          class="rounded-2xl shadow-2xl border-4 border-white object-cover w-full h-full"
        />
      </div>

    </div>
  </section>

    <section class="max-w-7xl mx-auto py-16 px-6">
      <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
        
        <div v-for="company in visibleCompanies" :key="company.name" class="bg-white rounded-xl shadow-sm border border-gray-100 overflow-hidden hover:shadow-xl transition-all group">
          
          <div class="h-32 bg-gray-200 relative">
            <img :src="company.bannerImage" class="w-full h-full object-cover" :alt="company.name + ' banner'" />
            <div class="absolute top-3 right-3 bg-[#10B981] text-white text-[10px] font-bold px-2 py-1 rounded uppercase">Premium</div>
          </div>

          <div class="p-6 pt-0 -mt-8 relative">
            <div class="w-16 h-16 bg-white border rounded shadow-sm overflow-hidden flex items-center justify-center mb-4">
              <img :src="company.logo" :alt="company.name" class="w-full h-full object-contain" />
            </div>

            <h3 class="text-lg font-bold">{{ company.name }}</h3>
            <p class="text-xs text-gray-500 mb-4">{{ company.industry }}</p>
            
            <a :href="company.profileUrl" class="inline-block w-full">
              <button class="w-full py-2 border-2 border-[#10B981] text-[#10B981] font-bold rounded hover:bg-[#10B981] hover:text-white transition-all uppercase text-xs">
                View Profile
              </button>
            </a>
          </div>
        </div>
      </div>

      <div v-if="hasMore" class="mt-12 flex justify-center">
        <button @click="loadMore" class="px-8 py-3 bg-[#1440b8] text-white font-bold rounded-lg hover:bg-blue-800 transition-colors shadow-lg">
          LOAD MORE COMPANIES
        </button>
      </div>
    </section>
  </div>
</template>