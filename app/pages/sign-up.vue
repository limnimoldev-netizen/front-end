<template>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/7.0.1/css/all.min.css">
  <div class="min-h-screen flex font-['Plus_Jakarta_Sans',sans-serif] selection:bg-indigo-500/30">


    <div class="hidden lg:block lg:flex-1 relative overflow-hidden bg-slate-950">
      <img 
        src="https://images.unsplash.com/photo-1542744173-8e7e53415bb0?auto=format&fit=crop&q=80&w=2070" 
        alt="Teamwork Collaboration"  
        class="absolute inset-0 w-full h-full object-cover object-center opacity-40 "
      />
      <div class="absolute inset-0 bg-gradient-to-tr "></div>
      
      <div class="absolute inset-0 flex flex-col justify-between p-16">
        <div class="flex justify-between items-start">
           
        </div>
        <div class="max-w-md">
           <div class="w-16 h-1 bg-indigo-500 mb-8 rounded-full"></div>
           <h2 class="text-6xl font-extrabold text-white leading-[1.1] mb-6">
            PEOPLE FIRST <br/> 
            <span class="text-indigo-400 ">SUCCESS ALWAYS</span>
          </h2>
          <p class="text-slate-400 text-sm">
            Join thousands of administrators managing the world's most dynamic talent streams.
          </p>
        </div>
      </div>
    </div>




    <main class="w-full lg:w-[45%] flex flex-col justify-center px-8 md:px-16 lg:px-20 bg-white relative z-10 overflow-y-auto">
      
      <div class="max-w-[500px] w-full mx-auto py-12">
        <router-link to="/" class="inline-flex items-center gap-3 mb-10 group">
<div class="w-11 h-11 flex items-center justify-center transition-all duration-300">
            <i class="fa-solid fa-arrow-left"></i>
          </div>
          <span class="text-l font-extrabold tracking-tighter text-slate-900  ">Back</span>
        </router-link>

        <div class="mb-8">
          <h1 class="text-4xl font-extrabold text-slate-900 tracking-tight">Create Account</h1>
          <p class="text-slate-500 mt-2 text-sm font-medium">Access your workspace. Manage your success.</p>
        </div>

        <form @submit.prevent="handleSignup" class="space-y-5">
          <div>
            <label class="block text-[10px] font-bold uppercase tracking-[0.2em] text-slate-400 mb-2 ml-1">Full Name</label>
            <input
              v-model="name"
              type="text"
              placeholder="John Doe"
              class="w-full bg-slate-50 border border-slate-200 rounded-2xl px-5 py-4 text-slate-900 transition-all focus:outline-none focus:border-indigo-600 focus:ring-4 focus:ring-indigo-600/5 placeholder:text-slate-300"
              required
            />
          </div>

          <div>
            <label class="block text-[10px] font-bold uppercase tracking-[0.2em] text-slate-400 mb-2 ml-1">Email Node</label>
            <input
              v-model="email"
              type="email"
              placeholder="name@example.com"
              class="w-full bg-slate-50 border border-slate-200 rounded-2xl px-5 py-4 text-slate-900 transition-all focus:outline-none focus:border-indigo-600 focus:ring-4 focus:ring-indigo-600/5 placeholder:text-slate-300"
              required
            />
          </div>

          <div>
            <label class="block text-[10px] font-bold uppercase tracking-[0.2em] text-slate-400 mb-2 ml-1">Create Security Key</label>
            <input
              v-model="password"
              type="password"
              placeholder="••••••••"
              class="w-full bg-slate-50 border border-slate-200 rounded-2xl px-5 py-4 text-slate-900 transition-all focus:outline-none focus:border-indigo-600 focus:ring-4 focus:ring-indigo-600/5 placeholder:text-slate-300"
              required
            />
          </div>

          <div>
            <label class="block text-[10px] font-bold uppercase tracking-[0.2em] text-slate-400 mb-2 ml-1">Verify Key</label>
            <input
              v-model="confirm"
              type="password"
              placeholder="••••••••"
              :class="{ 'border-rose-400 bg-rose-50': confirm && password !== confirm }"
              class="w-full bg-slate-50 border border-slate-200 rounded-2xl px-5 py-4 text-slate-900 transition-all focus:outline-none focus:border-indigo-600 focus:ring-4 focus:ring-indigo-600/5 placeholder:text-slate-300"
              required
            />
          </div>

          <button
            type="submit"
            :disabled="isLoading || (confirm && password !== confirm)"
            class="w-full mt-4 bg-[#1440b8] text-white font-bold uppercase text-[12px] tracking-[0.2em] py-5 rounded-2xl hover:bg-[#7087bb] transition-all duration-300 active:scale-[0.97] disabled:opacity-50 flex items-center justify-center gap-3 shadow-2xl shadow-indigo-900/10"
          >
            <span v-if="!isLoading">Register Node</span>
            <span v-else>Syncing to Database...</span>
            <i v-if="isLoading" class="fa-solid fa-circle-notch animate-spin text-indigo-300"></i>
          </button>
        </form>

        <Transition name="slide-up">
          <div v-if="message" :class="['mt-6 p-4 rounded-2xl text-center text-xs font-bold border', success ? 'bg-emerald-50 border-emerald-100 text-emerald-700' : 'bg-rose-50 border-rose-100 text-rose-600']">
            {{ message }}
          </div>
        </Transition>

        <div class="mt-10 pt-8 border-t border-slate-100 text-center">
          <p class="text-slate-400 text-xs font-medium">
            Already registered? 
            <router-link to="/login" class="text-[#1440b8] hover:text-[#7087bb] font-bold transition-colors ml-1">Login</router-link>
          </p>
        </div>
      </div>
    </main>

    

  </div>
</template>

<script setup>
import { ref } from "vue"
import { useRouter } from "vue-router"

const router = useRouter()
const name = ref("")
const email = ref("")
const password = ref("")
const confirm = ref("")
const message = ref("")
const success = ref(false)
const isLoading = ref(false)

async function handleSignup() {
  if (password.value !== confirm.value) {
    message.value = "Security Keys do not match."
    return
  }

  isLoading.value = true
  message.value = ""
  success.value = false

  try {
    const { data, error } = await supabase.auth.signUp({
      email: email.value,
      password: password.value,
      options: {
        data: {
          full_name: name.value,
        },
      },
    })

    if (error) throw error

    success.value = true
    message.value = "Account created! Redirecting to login..."
    
    setTimeout(() => {
      router.push("/login")
    }, 2000)

  } catch (error) {
    message.value = error.message || "An error occurred during registration."
    success.value = false
  } finally {
    isLoading.value = false
  }
}
</script>

<style scoped>
.slide-up-enter-active, 
.slide-up-leave-active { 
  transition: all 0.5s cubic-bezier(0.16, 1, 0.3, 1); 
}
.slide-up-enter-from { 
  opacity: 0; 
  transform: translateY(15px) scale(0.98); 
}

main {
  scrollbar-width: none;
}
main::-webkit-scrollbar {
  display: none;
}
</style>