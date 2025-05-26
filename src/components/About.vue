<template>
  <section class="py-16">
    <h2 class="text-3xl font-bold text-center mb-12">Tentang <span class="text-blue-600">Saya</span></h2>
    
    <div class="flex flex-col md:flex-row items-center gap-8">
      <div class="md:w-1/3 flex justify-center">
        <div class="w-64 h-64 rounded-full overflow-hidden border-4 border-blue-500">
          <img src="../assets/profile.jpeg" alt="Profile" class="w-full h-full object-cover">
        </div>
      </div>
      
      <div class="md:w-2/3">
        <h3 class="text-2xl font-semibold mb-4">Siapa Saya?</h3>
        <p class="text-gray-700 mb-6 leading-relaxed">
          Saya seorang pengembang frontend dengan spesialisasi dalam Vue.js. Saya memiliki pengalaman 3+ tahun dalam membangun aplikasi web yang responsif dan interaktif. Saya sangat tertarik dengan desain UI/UX dan selalu berusaha menciptakan pengalaman pengguna yang luar biasa. Selain itu saya juga berkembang di dunia backend di mana saya menggunakan Laravel ataupun hono sebagai rest full api
        </p>
        
        <div class="grid grid-cols-2 gap-4">
          <div>
            <h4 class="font-semibold">Nama:</h4>
            <p>Djumad Bantan</p>
          </div>
          <div>
            <h4 class="font-semibold">Email:</h4>
            <p>bantandjumad@gmail.com</p>
          </div>
          <div>
            <h4 class="font-semibold">Tanggal Lahir:</h4>
            <p>23 Maret 2003</p>
          </div>
          <div>
            <h4 class="font-semibold">Dari:</h4>
            <p>Ambon, Indonesia</p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>