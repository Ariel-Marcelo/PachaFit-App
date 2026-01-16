<script setup>
const products = [
  {
    id: 1,
    image: "/golden-flax-seeds-close-up-texture-food-photograph.jpg",
    alt: "Semillas de lino dorado",
  },
  {
    id: 2,
    image: "/green-mung-beans-close-up-texture-food-photography.jpg",
    alt: "Frijoles mungo verdes",
  },
  {
    id: 3,
    image: "/white-quinoa-seeds-close-up-texture-food-photograp.jpg",
    alt: "Semillas de quinoa blanca",
  },
  {
    id: 4,
    image: "/green-fennel-seeds-close-up-texture-food-photograp.jpg",
    alt: "Semillas de hinojo",
  },
  {
    id: 5,
    image: "/red-adzuki-beans-close-up-texture-food-photography.jpg",
    alt: "Frijoles adzuki rojos",
  },
  {
    id: 6,
    image: "/white-sesame-seeds-close-up-texture-food-photograp.jpg",
    alt: "Semillas de sésamo",
  },
]
</script>

<template>
  <div class="flex-1">
    <h2 class="text-2xl font-semibold text-[#3d4d3d] mb-6">Latest Arrivals</h2>

    <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-4">
      <div
          v-for="product in products"
          :key="product.id"
          class="group cursor-pointer"
      >
        <div class="rounded-2xl overflow-hidden bg-gray-100 aspect-square relative">
          <img
              :src="product.image || '/placeholder.svg'"
              :alt="product.alt"
              class="absolute inset-0 w-full h-full object-cover group-hover:scale-105 transition-transform duration-300"
              loading="lazy"
          />
        </div>
      </div>
    </div>
  </div>
</template>