<template>
  <section class="py-24">
    <div class="max-w-7xl px-2 sm:px-4 lg:px-6 mx-auto">
      <div class="grid grid-cols-1 xl:grid-cols-2 gap-8 items-center">
        <div class="flex flex-col gap-6">
          <p class="font-bold text-orange-300">O FIRMIE</p>
          <h1 class="font-bold text-5xl">
            Twój partner w
            <br />
            <span class="text-orange-300">transporcie ciężkim</span>
          </h1>
          <p>
            P.H.U. LEHMANN TRADE to firma z wieloletnim doświadczeniem w branży
            transportowej. Specjalizujemy się w transporcie ciężkim z
            wykorzystaniem nowoczesnych naczep oraz pojazdów marki Mercedes i
            Renault.
          </p>
          <p>
            Nasza siedziba znajduje się w Rybniku, skąd realizujemy zlecenia
            transportowe na terenie całej Polski i Europy. Stawiamy na jakość,
            bezpieczeństwo i terminowość każdej realizacji.
          </p>

          <div
            class="flex w-fit gap-4 p-4 bg-gray-100 rounded-2xl items-center"
          >
            <Icon icon="award" />

            <div class="flex flex-col py-1">
              <h3 class="font-bold">P.H.U. LEHMANN TRADE</h3>
              <p class="text-sm text-gray-600">NIP: 642-288-51-36</p>
            </div>
          </div>
        </div>

        <div
          class="grid grid-cols-1 md:grid-cols-2 gap-x-4 gap-y-4 justify-start"
        >
          <Card
            icon="shield"
            title="Bezpieczeństwo"
            desc="Najwyższe standardy bezpieczeństwa przewozu ładunków"
          />
          <Card
            icon="clock"
            title="Punktualność"
            desc="Terminowa realizacja każdego zlecenia transportowego"
          />
          <Card
            icon="users"
            title="Doświadczenie"
            desc="Wykwalifikowana kadra kierowców z wieloletnim stażem"
          />
          <Card
            icon="award"
            title="Profesjonalizm"
            desc="Kompleksowa obsługa i indywidualne podejście do klienta"
          />
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import Card from "./Card.vue";
import Icon from "./Icon.vue";
</script>
