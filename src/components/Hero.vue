<template>
  <section
    class="relative min-h-screen bg-cover bg-center"
    style="background-image: url(&quot;/nightXL.jpg&quot;)"
  >
    <div class="absolute inset-0 bg-black/60"></div>

    <div
      class="relative z-10 flex flex-col items-center justify-center min-h-screen text-center px-4"
    >
      <div class="max-w-3xl text-white mx-auto">
        <Badge
          text="Transport ciężki z naczepami"
          showIcon
          bg="bg-amber-400/40"
          border="border-amber-500"
          textColor="text-amber-500"
        />

        <h1
          class="text-4xl sm:text-5xl md:text-7xl font-extrabold leading-tight"
        >
          LEHMANN <br />
          <span class="text-amber-300">TRADE</span>
        </h1>

        <p class="mt-6 text-lg sm:text-xl text-white/90">
          Profesjonalny transport ciężki na terenie całej Europy
        </p>

        <p class="mt-2 text-sm text-white/70">
          Flota Mercedes & Renault • Naczepy • Doświadczenie od lat
        </p>

        <div class="mt-8 flex flex-col sm:flex-row gap-6 justify-center">
          <Button
            text="Skontaktuj się"
            icon="phone"
            class="px-8 py-4 text-lg"
            hoverable
          />

          <Button
            text="Zobacz flotę"
            icon="truck"
            class="px-8 py-4 text-lg"
            hoverable
          />
        </div>

        <div class="mt-12 grid grid-cols-3 gap-20">
          <div>
            <p class="text-5xl font-bold text-amber-300 p-2">15+</p>

            <p class="text-sm text-white/70">Lat doświadczenia</p>
          </div>
          <div>
            <p class="text-5xl font-bold text-amber-300 p-2">EU</p>
            <p class="text-sm text-white/70">Zasięg działania</p>
          </div>
          <div>
            <p class="text-5xl font-bold text-amber-300 p-2">24/7</p>
            <p class="text-sm text-white/70">Dostępność</p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
<script setup>
import Button from "./Button.vue";
import Badge from "./Badge.vue";
</script>
