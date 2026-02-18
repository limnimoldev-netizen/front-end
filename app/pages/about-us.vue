<template>


  <div class="min-h-screen bg-[#F8FAFC] text-[#000001] font-sans">
     

      <section class="py-16 px-5 text-center">
          <h2 class="text-5xl font-extrabold mb-4">Building Solutions</h2>
          <p class="text-xl text-gray-600">Innovative ideas for a better tomorrow.</p>
    </section>



    <section class="py-12 px-5 max-w-6xl mx-auto">

         <h2 class="text-3xl font-bold text-center mb-10">Meet Our Leaders</h2>
      
         <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-8">

         <div v-for="member in team" :key="member.name" class="bg-white p-6 rounded-lg shadow-md text-center border border-gray-200">
          
         <div class="mb-4 flex justify-center">

            <img v-if="member.image" :src="member.image" class="w-32 h-32 rounded-full object-cover border-2 border-[#1440b8]" alt="profile">
            <div v-else class="w-32 h-32 rounded-full bg-[#1440b8] text-white flex items-center justify-center text-2xl font-bold">
              {{ member.initials }}
            </div>
          </div>

          <h3 class="text-xl font-bold">{{ member.name }}</h3>
          <p class="text-[#1440b8] font-medium mb-2">{{ member.role }}</p>
          <p class="text-sm text-gray-500 leading-snug">{{ member.bio }}</p>
        </div>
      </div>
    </section>

    <section class="bg-gray-100 py-12 border-y border-gray-300">
      <div class="max-w-4xl mx-auto grid grid-cols-2 md:grid-cols-4 gap-4 text-center">
        <div v-for="stat in stats" :key="stat.label">
          <div class="text-3xl font-bold text-[#1440b8]">{{ stat.number }}</div>
          <div class="text-gray-600 text-sm">{{ stat.label }}</div>
        </div>
      </div>
    </section>
    <section class="py-20 px-6 bg-white">
  <div class="container mx-auto max-w-4xl text-center">
    <h2 class="text-3xl font-bold text-blue-800 mb-6">Our Mission</h2>
    <p class="text-gray-600 leading-relaxed mb-6 italic text-lg">
      "It started with a simple observation: the bridge between talent and opportunity was broken."
    </p>
    <p class="text-gray-600 leading-relaxed">
      Founded in 2024, PeopleCore HR began as a small project to help local businesses in Asia navigate the complexities of digital hiring. We realized that while technology was advancing, the 'human' element was being lost in automated systems. We built this platform to bring that balance back—giving recruiters powerful tools while treating every applicant as a person, not just a resume.
    </p><br><br>
     <h2 class="text-3xl font-bold text-blue-800 mb-6">Our Vision</h2>
   
    <p class="text-gray-600 leading-relaxed mb-6">
      We aim to become the most trusted HR technology platform in Asia, connecting people and companies through innovation,
      understanding, and transparency. By combining smart tools with human care, we make hiring and job searching simple,
      accessible, and meaningful for all.
    </p>
   
  </div>
</section>
<section class="bg-gray-50 py-20 px-6">
  <div class="container mx-auto max-w-6xl grid md:grid-cols-2 gap-10 items-center">
    <!-- ✅ Left: Contact Info -->
    <div class="text-left space-y-5">
      <h2 class="text-3xl font-bold text-blue-800 mb-2">Get in Touch</h2>
      <p class="text-gray-600 mb-6">
        We’re here to help you connect with the right opportunities.  
        Reach out to us for recruitment support, partnership, or any inquiries.
      </p>

      <div class="space-y-3 text-gray-700">
        <p>
          <span class="font-semibold text-black-700">Company:</span>
          PeopleCore HR Solutions
        </p>
        <p>
          <span class="font-semibold text-black-700">Address:</span>
          #23, Street 200, Phnom Penh, Cambodia
        </p>
        <p>
          <span class="font-semibold text-black-700">Phone:</span>
          +855 96 123 4567
        </p>
        <p>
          <span class="font-semibold text-black-700">Email:</span>
          <a
            href="mailto:info@peoplecorehr.com"
            class="text-blue-600 hover:underline"
          >
            info@peoplecorehr.com
          </a>
        </p>
        <p>
          <span class="font-semibold text-black-700">Website:</span>
          <a
            href="https://peoplecorehr.com"
            class="text-blue-600 hover:underline"
            target="_blank"
          >
            www.peoplecorehr.com
          </a>
        </p>
      </div>
    </div>

    <!-- ✅ Right: Google Map -->
    <div class="rounded-lg overflow-hidden shadow-lg">
      <iframe
        class="w-full h-80 md:h-[400px]"
        src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3919.508067476034!2d104.91870277474803!3d11.549999088662178!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x3109512c16c3662d%3A0x9e5c7989b7de8f6a!2sPhnom%20Penh%2C%20Cambodia!5e0!3m2!1sen!2skh!4v1700000000000!5m2!1sen!2skh"
        style="border:0;"
        allowfullscreen=""
        loading="lazy"
        referrerpolicy="no-referrer-when-downgrade"
      ></iframe>
    </div>
  </div>
</section>



<section class="py-20 px-6 bg-blue-50">
  <div class="container mx-auto">
    <h2 class="text-3xl font-bold text-center text-blue-800 mb-12">How It Works</h2>
    <div class="grid md:grid-cols-4 gap-6 text-center">
      <div class="p-4">
        <div class="text-2xl font-bold text-blue-600 mb-2">01</div>
        <h4 class="font-bold mb-2">Create Profile</h4>
        <p class="text-sm text-gray-500">Candidates upload CVs and showcase their best skills.</p>
      </div>
      <div class="p-4">
        <div class="text-2xl font-bold text-blue-600 mb-2">02</div>
        <h4 class="font-bold mb-2">Smart Matching</h4>
        <p class="text-sm text-gray-500">Our system connects you with roles that actually fit.</p>
      </div>
      <div class="p-4">
        <div class="text-2xl font-bold text-blue-600 mb-2">03</div>
        <h4 class="font-bold mb-2">Direct Interview</h4>
        <p class="text-sm text-gray-500">Schedule and meet through our integrated platform.</p>
      </div>
      <div class="p-4">
        <div class="text-2xl font-bold text-blue-600 mb-2">04</div>
        <h4 class="font-bold mb-2">Get Hired</h4>
        <p class="text-sm text-gray-500">Seamless onboarding into your new dream career.</p>
      </div>
    </div>
  </div>
</section>

    <footer class="bg-[#F8FAFC] py-16 text-center">
      <h2 class="text-2xl font-bold mb-6">Ready to join us?</h2>
      
      <button class="bg-[#1440b8] hover:bg-[#7087bb] text-white px-8 py-3 rounded mr-4 transition-colors">
        Get In Touch
      </button>

      <button class="bg-[#10B981] hover:opacity-90 text-white px-8 py-3 rounded transition-opacity">
        Apply Now
      </button>
    </footer>
  </div>
</template>

<script setup>
// Simplified Data Arrays
const team = [
  {
    name: 'justin in khmer',
    role: 'CEO & Founder',
    initials: 'SJ',
    image: 'https://i.ibb.co/JZcjp4h/dara.jpg', // Replace with your actual image link
    bio: 'Visionary leader with 15+ years of experience in tech innovation.'
  },
  {
    name: 'Daniel Loeu walker',
    role: 'CTO',
    initials: 'MC',
    image: 'https://i.ibb.co/xdKpky6/loeu-pro.jpg', // Empty means it will show the initials (MC)
    bio: 'Tech enthusiast passionate about building scalable solutions.'
  },
  {
    name: 'Elise molly pav',
    role: 'Head of Design',
    initials: 'ER',
    image: 'https://i.ibb.co/7xVLDmcR/broooo-pav.jpg',
    bio: 'Creative mind dedicated to crafting beautiful user experiences.'
  },
  {
    name: 'Pichie lewandovskie',
    role: 'Lead Developer',
    initials: 'DT',
    image: 'https://i.ibb.co/gndJP2c/pich-boss.jpg',
    bio: 'Full-stack developer who loves turning ideas into reality.'
  }
];
const stats = [
  { number: '500+', label: 'Projects' },
  { number: '200+', label: 'Clients' },
  { number: '50+', label: 'Team' },
  { number: '10+', label: 'Years' }
];
</script>