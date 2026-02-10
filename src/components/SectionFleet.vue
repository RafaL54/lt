<template>
  <section class="py-24 bg-gray-100">
    <div class="max-w-7xl px-2 sm:px-4 lg:px-6 mx-auto">
      <div class="flex flex-col gap-6 text-center font-semibold">
        <p class="text-amber-400">NASZA FLOTA</p>
        <h2 class="text-5xl">Nowoczesne pojazdy</h2>
        <h3 class="text-lg font-normal max-w-2xl mx-auto">
          Dysponujemy flotą nowoczesnych ciągników siodłowych marek
          Mercedes-Benz oraz Renault wraz z profesjonalnymi naczepami
        </h3>
        <div
          class="grid grid-cols-1 md:grid-cols-2 md:grid-rows-[auto_auto] gap-6 pt-6"
        >
          <div class="bg-white rounded-2xl shadow overflow-hidden">
            <div
              class="relative h-64 bg-cover bg-center"
              style="background-image: url(&quot;/truck.jpg&quot;)"
            >
              <div class="absolute inset-0 bg-black/40"></div>

              <div
                class="absolute bottom-4 left-4 z-10 text-white max-w-xs text-left"
              >
                <p class="text-sm">Mercedes-Benz</p>
                <h3 class="text-3xl font-bold">Actros</h3>
              </div>
            </div>

            <div class="flex flex-wrap gap-2 p-6 rounded-b-2xl text-sm">
              <Badge text="Nowoczesne naczepy" />
              <Badge text="System GPS" />
              <Badge text="Klimatyzacja" />
              <Badge text="Euro 6" />
            </div>
          </div>

          <div class="bg-white rounded-2xl shadow overflow-hidden">
            <div
              class="relative h-64 bg-cover bg-center"
              style="background-image: url(&quot;/truck.jpg&quot;)"
            >
              <div class="absolute inset-0 bg-black/40"></div>

              <div
                class="absolute bottom-4 left-4 z-10 text-white max-w-xs text-left"
              >
                <p class="text-sm">Renault</p>
                <h3 class="text-3xl font-bold">T-Series</h3>
              </div>
            </div>

            <div class="flex flex-wrap gap-2 p-6 rounded-b-2xl text-sm">
              <Badge text="Duża ładowność" />
              <Badge text="Ekonomiczny" />
              <Badge text="Niezawodny" />
              <Badge text="Euro 6" />
            </div>
          </div>

          <div
            class="bg-white/70 text-black/70 p-6 mt-8 rounded-2xl shadow md:col-span-2"
          >
            <div
              class="grid grid-cols-1 md:grid-cols-4 gap-x-4 gap-y-4 justify-start"
            >
              <Card
                icon="shield"
                title="Naczepy"
                desc="Standardowe i specialistyczne"
                bgClass="bg-transparent"
                hoverClass=""
                iconPosition="center"
                class="text-xl"
              />
              <Card
                icon="shield"
                title="Ładowność"
                desc="Do 24 ton"
                bgClass="bg-transparent"
                hoverClass=""
                iconPosition="center"
                class="text-xl"
              />
              <Card
                icon="shield"
                title="Ubezpieczenie"
                desc="Pełne OCP"
                bgClass="bg-transparent"
                hoverClass=""
                iconPosition="center"
                class="text-xl"
              />
              <Card
                icon="shield"
                title="Norma"
                desc="Euro 6"
                bgClass="bg-transparent"
                hoverClass=""
                iconPosition="center"
                class="text-xl"
              />
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
<script setup>
import Card from "./Card.vue";
import Badge from "./Badge.vue";
</script>
