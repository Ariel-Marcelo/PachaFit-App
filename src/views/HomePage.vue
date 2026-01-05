<template>
  <ion-page>
    <ion-content>
      <div class="flex flex-col items-center justify-center min-h-screen p-6 bg-slate-50">

        <div class="w-full max-w-sm p-8 bg-white shadow-2xl rounded-[--radius-pacha] border border-slate-100">
          <div class="flex items-center justify-between mb-6">
            <h1 class="text-3xl font-black text-[--color-pacha-dark] italic">PACHA FIT</h1>
            <div class="w-3 h-3 bg-[--color-pacha-main] rounded-full animate-ping"></div>
          </div>

          <p class="mb-8 text-slate-500 text-pretty">
            Tu transformación comienza hoy. Registra tu actividad y alcanza tus metas.
          </p>
          <div class="bg-pacha-main text-pacha-dark rounded-pacha">
            Contenido con colores correctos
          </div>

          <button class="w-full py-4 font-bold text-white transition-all bg-[--color-pacha-main] rounded-2xl active:scale-95 shadow-lg shadow-emerald-200">
            EMPEZAR AHORA
          </button>
        </div>

      </div>
    </ion-content>
  </ion-page>
</template>

<script setup lang="ts">
import { IonPage, IonContent } from '@ionic/vue';
/* Al usar TS, WebStorm te dará autocompletado total aquí */
</script>