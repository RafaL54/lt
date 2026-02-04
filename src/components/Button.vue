<template>
  <button
    class="flex items-center gap-2 px-4 py-2 rounded-2xl cursor-pointer transition-colors duration-200"
    :class="[
      bg,
      textColor,
      hoverable ? hoverBg : '',
      hoverable ? hoverText : '',
    ]"
  >
    <!-- Ikona PHONE -->
    <svg
      v-if="icon === 'phone'"
      xmlns="http://www.w3.org/2000/svg"
      width="20"
      height="20"
      viewBox="0 0 24 24"
      fill="none"
      stroke="currentColor"
      stroke-width="2"
      stroke-linecap="round"
      stroke-linejoin="round"
    >
      <path
        d="M13.832 16.568a1 1 0 0 0 1.213-.303l.355-.465A2 2 0 0 1 17 15h3a2 2 0 0 1 2 2v3a2 2 0 0 1-2 2A18 18 0 0 1 2 4a2 2 0 0 1 2-2h3a2 2 0 0 1 2 2v3a2 2 0 0 1-.8 1.6l-.468.351a1 1 0 0 0-.292 1.233 14 14 0 0 0 6.392 6.384"
      />
    </svg>

    <!-- Ikona TRUCK -->
    <svg
      v-else-if="icon === 'truck'"
      xmlns="http://www.w3.org/2000/svg"
      width="20"
      height="20"
      viewBox="0 0 24 24"
      fill="none"
      stroke="currentColor"
      stroke-width="2"
      stroke-linecap="round"
      stroke-linejoin="round"
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
  </button>
</template>

<script setup>
const props = defineProps({
  text: String,
  icon: { type: String, default: "" },
  hoverable: { type: Boolean, default: false }, // <--- tutaj opcja
});

// Normalne kolory
const bg =
  props.icon === "phone"
    ? "bg-orange-400"
    : props.icon === "truck"
      ? "bg-white"
      : "bg-orange-400";
const textColor =
  props.icon === "phone"
    ? "text-black"
    : props.icon === "truck"
      ? "text-gray-700"
      : "text-black";

// Kolory po hover
const hoverBg =
  props.icon === "phone"
    ? "hover:bg-orange-500"
    : props.icon === "truck"
      ? "hover:bg-gray-200"
      : "hover:bg-orange-500";
const hoverText =
  props.icon === "phone"
    ? "hover:text-white"
    : props.icon === "truck"
      ? "hover:text-black"
      : "hover:text-white";
</script>
