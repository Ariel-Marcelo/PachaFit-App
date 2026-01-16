<template>
  <ion-page>
    <ion-content :fullscreen="true">
      <div class="min-h-screen bg-[#d4b8a0]">
        <header-nav></header-nav>
        <hero-section></hero-section>

        <div class="bg-white rounded-t-[40px] -mt-8 relative z-10 min-h-screen">
          <div class="max-w-7xl mx-auto px-6 py-10">
            <div class="flex flex-col md:flex-row gap-8">
              <CategoriesSidebar />
              <LatestArrivals />
            </div>
          </div>
        </div>
      </div>
    </ion-content>
  </ion-page>
</template>

<script setup lang="ts">
import { IonPage, IonContent } from '@ionic/vue';
import HeaderNav from "@/components/HeaderNav.vue";
import HeroSection from "@/components/HeroSection.vue";
import CategoriesSidebar from "@/components/CategoriesSidebar.vue";
import LatestArrivals from "@/components/LatestArrivals.vue";
</script>

<style scoped>
ion-content {
  --background: #d4b8a0;
}
</style>