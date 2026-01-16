<template>
  <header class="bg-[#f5ebe0] px-6 py-4">
    <div class="max-w-7xl mx-auto flex items-center justify-between gap-4">
      <div class="flex-shrink-0">
        <svg width="50" height="60" viewBox="0 0 50 60" fill="none" xmlns="http://www.w3.org/2000/svg">
          <path d="M25 5C25 5 15 15 15 25C15 30 18 35 25 35C32 35 35 30 35 25C35 15 25 5 25 5Z" fill="#4a5d4a" />
          <path d="M25 20C25 20 20 25 20 30C20 33 22 36 25 36C28 36 30 33 30 30C30 25 25 20 25 20Z" fill="#3d4d3d" />
          <path d="M25 35V55" stroke="#4a5d4a" stroke-width="3" stroke-linecap="round" />
          <path
              d="M20 45C20 45 22 42 25 42C28 42 30 45 30 45"
              stroke="#4a5d4a"
              stroke-width="2"
              stroke-linecap="round"
          />
          <path
              d="M18 50C18 50 21 47 25 47C29 47 32 50 32 50"
              stroke="#4a5d4a"
              stroke-width="2"
              stroke-linecap="round"
          />
        </svg>
      </div>

      <div class="flex-1 max-w-2xl">
        <div class="relative flex items-center">
          <input
              type="text"
              placeholder=""
              class="w-full bg-[#f0e6d9] rounded-full py-3 pl-6 pr-14 text-[#5a6b5a] placeholder-[#8a9b8a] focus:outline-none focus:ring-2 focus:ring-[#5a6b5a]/30"
          />
          <button class="absolute right-1 bg-white rounded-full p-3 shadow-sm hover:shadow-md transition-shadow">
            <Search class="w-5 h-5 text-[#5a6b5a]" />
          </button>
        </div>
      </div>

      <div class="flex items-center gap-4">
        <button class="bg-[#c17d6a] text-white px-8 py-3 rounded-full font-medium hover:bg-[#a86b5a] transition-colors">
          Sign In
        </button>

        <button class="p-2 hover:bg-[#e8ddd0] rounded-full transition-colors">
          <User class="w-8 h-8 text-[#5a6b5a]" :size="32" :stroke-width="1.5" />
        </button>

        <button class="p-2 hover:bg-[#e8ddd0] rounded-full transition-colors relative">
          <ShoppingCart class="w-8 h-8 text-[#5a6b5a]" :size="32" :stroke-width="1.5" />
          <span class="absolute -top-1 -right-1 bg-[#c17d6a] text-white text-xs w-5 h-5 rounded-full flex items-center justify-center font-medium">
            3
          </span>
        </button>
      </div>

    </div>
  </header>
</template>

<script setup>
import { Search, ShoppingCart, User } from 'lucide-vue-next'
</script>