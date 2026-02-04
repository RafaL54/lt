<template>
  <header class="fixed top-0 left-0 w-full z-50 backdrop-blur-md shadow-md">
    <div class="max-w-7xl mx-auto flex justify-between items-center p-4">
      <a href="#" class="flex items-center gap-2">
        <Logo />
      </a>

      <nav class="hidden md:flex gap-8 items-center text-white">
        <a href="#o-firmie" class="hover:text-amber-300 py-3">O Firmie</a>
        <a href="#flota" class="hover:text-amber-300 py-3">Flota</a>
        <a href="#uslugi" class="hover:text-amber-300 py-3">Usługi</a>
        <a href="#kontakt" class="hover:text-amber-300 py-3">Kontakt</a>
        <Button
          text="Zadzwoń"
          icon="phone"
          class="px-6 py-3 text-md hover:bg-amber-200"
        />
      </nav>
    </div>
  </header>
</template>
<script setup>
import Logo from "./Logo.vue";
import Button from "./Button.vue";
</script>

<style scoped></style>
