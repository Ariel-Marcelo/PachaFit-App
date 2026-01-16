<script setup>
import { ref } from 'vue'
import { Heart, ChevronRight } from 'lucide-vue-next'

const categories = [
  { id: 1, name: "Heat Q/a.s 500K" },
  { id: 2, name: "Grains & Seeds" },
  { id: 3, name: "Dried Fruits" },
  { id: 4, name: "Cleaning Essentials" },
  { id: 5, name: "Personal Care" },
]

// Estado reactivo para la categoría activa
const activeCategory = ref(1)

const setActiveCategory = (id) => {
  activeCategory.value = id
}
</script>

<template>
  <div class="w-72 flex-shrink-0">
    <div class="bg-gradient-to-b from-[#c8d4c4] to-[#9aab97] rounded-3xl p-6 shadow-lg">

      <div class="flex justify-center mb-6">
        <div class="bg-white/30 p-3 rounded-full">
          <Heart class="w-6 h-6 text-[#5a6b5a]" :stroke-width="1.5" />
        </div>
      </div>

      <h2 class="text-xl font-semibold text-[#3d4d3d] mb-4">Categories</h2>

      <nav class="space-y-2">
        <button
            v-for="category in categories"
            :key="category.id"
            @click="setActiveCategory(category.id)"
            :class="[
            'w-full flex items-center justify-between px-4 py-3 rounded-full transition-all',
            activeCategory === category.id
              ? 'bg-[#5a6b5a] text-white'
              : 'text-[#3d4d3d] hover:bg-white/20'
          ]"
        >
          <span class="font-medium text-sm">{{ category.name }}</span>
          <ChevronRight class="w-4 h-4" />
        </button>
      </nav>

    </div>
  </div>
</template>