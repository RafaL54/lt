<template>
  <span
    class="inline-flex items-center gap-1 px-3 py-1 rounded-full border"
    :class="[bg, border, textColor]"
  >
    <!-- Ikona truck tylko jeśli showIcon = true -->
    <svg
      v-if="showIcon"
      xmlns="http://www.w3.org/2000/svg"
      width="16"
      height="16"
      viewBox="0 0 24 24"
      fill="none"
      stroke="currentColor"
      stroke-width="2"
      stroke-linecap="round"
      stroke-linejoin="round"
      class="mr-1"
    >
      <path d="M14 18V6a2 2 0 0 0-2-2H4a2 2 0 0 0-2 2v11a1 1 0 0 0 1 1h2" />
      <path d="M15 18H9" />
      <path
        d="M19 18h2a1 1 0 0 0 1-1v-3.65a1 1 0 0 0-.22-.624l-3.48-4.35A1 1 0 0 0 17.52 8H14"
      />
      <circle cx="17" cy="18" r="2" />
      <circle cx="7" cy="18" r="2" />
    </svg>

    {{ text }}
  </span>
</template>

<script setup>
const props = defineProps({
  text: { type: String, required: true },
  showIcon: { type: Boolean, default: false },

  // kolory Tailwind
  bg: { type: String, default: "bg-gray-100" }, // tło
  border: { type: String, default: "border-gray-300" }, // cienka ramka
  textColor: { type: String, default: "text-black" }, // kolor tekstu + ikony
});
</script>
