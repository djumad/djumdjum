<template>
  <section class="py-16 bg-gray-100">
    <div class="container mx-auto px-4 max-w-4xl">
      <h2 class="text-3xl font-bold text-center mb-4">Hubungi <span class="text-purple-600">Saya</span></h2>
      <p class="text-center text-gray-600 mb-12">Silakan hubungi saya melalui formulir di bawah ini</p>
      
      <form class="bg-white p-8 rounded-lg shadow-md">
        <div class="grid grid-cols-1 md:grid-cols-2 gap-6 mb-6">
          <div>
            <label for="name" class="block text-gray-700 mb-2">Nama Lengkap</label>
            <input type="text" id="name" class="w-full px-4 py-2 border rounded-lg focus:outline-none focus:ring-2 focus:ring-purple-500">
          </div>
          <div>
            <label for="email" class="block text-gray-700 mb-2">Email</label>
            <input type="email" id="email" class="w-full px-4 py-2 border rounded-lg focus:outline-none focus:ring-2 focus:ring-purple-500">
          </div>
        </div>
        
        <div class="mb-6">
          <label for="subject" class="block text-gray-700 mb-2">Subjek</label>
          <input type="text" id="subject" class="w-full px-4 py-2 border rounded-lg focus:outline-none focus:ring-2 focus:ring-purple-500">
        </div>
        
        <div class="mb-6">
          <label for="message" class="block text-gray-700 mb-2">Pesan</label>
          <textarea id="message" rows="5" class="w-full px-4 py-2 border rounded-lg focus:outline-none focus:ring-2 focus:ring-purple-500"></textarea>
        </div>
        
        <button type="submit" class="w-full bg-purple-600 text-white py-3 rounded-lg font-bold hover:bg-purple-700 transition">
          Kirim Pesan
        </button>
      </form>
    </div>
  </section>
</template>