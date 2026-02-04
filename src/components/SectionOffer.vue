<template>
  <section class="py-24 bg-white">
    <div class="max-w-7xl px-4 mx-auto">
      <div class="text-center mb-12">
        <p class="text-amber-400 font-semibold">USŁUGI</p>
        <h2 class="text-5xl font-bold mt-2">Co oferujemy</h2>
        <p class="text-lg text-black/70 max-w-2xl mx-auto mt-4">
          Kompleksowe usługi transportowe dostosowane do indywidualnych potrzeb
          każdego klienta
        </p>
      </div>

      <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
        <Card
          icon="shield"
          title="Wsparcie 24/7"
          desc="Całodobowa obsługa klienta i monitoring realizowanych zleceń."
        />

        <Card
          icon="clock"
          title="Transport krajowy"
          desc="Realizacja zleceń transportowych na terenie całej Polski z gwarancją terminowości."
        />

        <Card
          icon="clock"
          title="Transport międzynarodowy"
          desc="Przewozy na terenie Europy z pełną dokumentacją i odprawą celną."
        />

        <Card
          icon="award"
          title="Transport z naczepami"
          desc="Specjalistyczne naczepy dostosowane do różnych typów ładunków."
        />

        <Card
          icon="users"
          title="Terminowe dostawy"
          desc="Punktualne realizacje z możliwością śledzenia przesyłki w czasie rzeczywistym."
        />

        <Card
          icon="shield"
          title="Pełna dokumentacja"
          desc="Kompletna obsługa dokumentacyjna i formalności transportowe."
        />

        <div
          class="md:col-span-3 mt-6 p-10 bg-black/40 rounded-2xl flex flex-col items-center text-center gap-6"
        >
          <h2 class="text-4xl text-white font-semibold">
            Potrzebujesz transportu?
          </h2>

          <p class="text-white/80 max-w-2xl">
            Skontaktuj się z nami, a przygotujemy indywidualną ofertę dopasowaną
            do Twoich potrzeb.
          </p>

          <Button
            text="Zapytaj o wycenę"
            class="px-8 py-4 text-lg shadow-xl hover:scale-105 transition-transform duration-200"
          />
        </div>
      </div>
    </div>
  </section>
</template>
<script setup>
import Card from "./Card.vue";
import Button from "./Button.vue";
</script>
