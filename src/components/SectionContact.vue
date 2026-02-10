<template>
  <section class="py-24 bg-gray-100">
    <div class="max-w-7xl px-4 mx-auto">
      <div class="text-center mb-12">
        <p class="text-amber-400 font-semibold">KONTAKT</p>
        <h2 class="text-5xl font-bold mt-2">Skontaktuj się z nami</h2>
        <p class="text-lg text-black/70 max-w-2xl mx-auto mt-4">
          Masz pytania? Chcesz poznać ofertę transportową? Wypełnij formularz
          lub skontaktuj się z nami bezpośrednio.
        </p>
      </div>

      <div class="grid grid-cols-1 lg:grid-cols-2 gap-8 items-stretch">
        <div class="flex flex-col gap-6 h-full">
          <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
            <Card
              icon="shield"
              title="Bezpieczeństwo"
              desc="Najwyższe standardy transportu"
              bgClass="bg-gray-200 text-black"
            />
            <Card
              icon="clock"
              title="Punktualność"
              desc="Terminowa realizacja zleceń"
              bgClass="bg-gray-200 text-black"
            />
            <Card
              icon="users"
              title="Doświadczenie"
              desc="Wykwalifikowana kadra kierowców"
              bgClass="bg-gray-200 text-black"
            />
            <Card
              icon="award"
              title="Profesjonalizm"
              desc="Kompleksowa obsługa klienta"
              bgClass="bg-gray-200 text-black"
            />
          </div>

          <form class="mt-6 flex flex-col gap-4 flex-1">
            <input
              type="text"
              placeholder="Imię i nazwisko"
              class="border rounded-lg p-3 w-full"
            />
            <input
              type="tel"
              placeholder="Telefon"
              class="border rounded-lg p-3 w-full"
            />
            <input
              type="email"
              placeholder="E-mail"
              class="border rounded-lg p-3 w-full"
            />
            <textarea
              placeholder="Wiadomość"
              class="border rounded-lg p-3 w-full"
              rows="5"
            ></textarea>

            <Button
              text="Wyślij wiadomość"
              icon="phone"
              class="w-full px-6 py-4 text-lg font-semibold shadow-xl hover:scale-105 transition-transform duration-200"
            />
          </form>
        </div>

        <div class="flex flex-col h-full rounded-2xl overflow-hidden shadow-xl">
          <div
            class="bg-white/90 backdrop-blur-md p-4 flex items-center gap-3 border-b border-black/10"
          >
            <svg
              xmlns="http://www.w3.org/2000/svg"
              class="w-6 h-6 text-amber-400"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
              stroke-width="2"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                d="M17.657 16.657L13 21.314l-4.657-4.657A8 8 0 1117.657 16.657z"
              />
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                d="M15 11a3 3 0 11-6 0 3 3 0 016 0z"
              />
            </svg>

            <div class="flex flex-col">
              <span class="font-semibold text-lg">Nasza lokalizacja</span>
              <span class="text-gray-700 text-sm">
                ul. Pod Lasem 68E, 44-210 Rybnik
              </span>
            </div>
          </div>

          <iframe
            src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2563.804820348333!2d18.512753215998114!3d50.10528877942959!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x4710fcd14f1b5673%3A0x1234567890abcdef!2sRybnik%2C%20Poland!5e0!3m2!1sen!2sus!4v1670000000000!5m2!1sen!2sus"
            class="w-full flex-1 border-0"
            loading="lazy"
            referrerpolicy="no-referrer-when-downgrade"
          ></iframe>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import Card from "./Card.vue";
import Button from "./Button.vue";
</script>
