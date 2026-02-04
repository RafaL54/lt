<template>
  <footer class="bg-black text-white p-16">
    <div class="max-w-7xl mx-auto px-4">
      <div class="grid grid-cols-1 md:grid-cols-3 gap-10 pb-12">
        <div class="flex flex-col gap-4">
          <Logo />

          <p class="text-white/70 text-sm leading-relaxed max-w-sm">
            Profesjonalny transport ciężki z naczepami. Mercedes & Renault.
            Polska i Europa.
          </p>
        </div>

        <div>
          <h4 class="font-semibold mb-4">Nawigacja</h4>
          <ul class="flex flex-col gap-2 text-white/70 text-sm">
            <li><a href="#o-nas" class="hover:text-amber-400">O nas</a></li>
            <li><a href="#flota" class="hover:text-amber-400">Flota</a></li>
            <li><a href="#uslugi" class="hover:text-amber-400">Usługi</a></li>
            <li><a href="#kontakt" class="hover:text-amber-400">Kontakt</a></li>
          </ul>
        </div>

        <div>
          <h4 class="font-semibold mb-4">Kontakt</h4>
          <div
            class="flex flex-col gap-2 text-white/70 text-sm leading-relaxed"
          >
            <p>Tel: 32 42 48 759</p>
            <p>Kom: 508 825 120</p>
            <p>E-mail: biuro@lehmann-trade.com</p>

            <p class="mt-2">
              ul. Pod Lasem 68E<br />
              44-210 Rybnik
            </p>
          </div>
        </div>
      </div>

      <div class="border-t border-white/10"></div>

      <div class="py-6 text-center text-sm text-white/50">
        <p>© 2026 P.H.U. LEHMANN TRADE. Wszelkie prawa zastrzeżone.</p>

        <p class="mt-2">NIP: 642-288-51-36 | REGON: 241953526</p>
      </div>
    </div>
  </footer>
</template>
<script setup>
import Logo from "./Logo.vue";
</script>
