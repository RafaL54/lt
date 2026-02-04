<template>
  <div
    :class="[
      'flex flex-col gap-2 p-4 rounded-2xl transition',
      bgClass,
      hoverClass,
    ]"
  >
    <Icon
      v-if="icon"
      :icon="icon"
      :class="[
        iconPosition === 'left' ? 'self-start' : 'self-center',
        iconColorClass,
      ]"
    />

    <h3 class="font-semibold">
      {{ title }}
    </h3>

    <p class="text-sm">
      {{ desc }}
    </p>
  </div>
</template>

<script setup>
import Icon from "./Icon.vue";

defineProps({
  title: String,
  desc: String,
  icon: String,

  /* KOLORY */
  bgClass: {
    type: String,
    default: "bg-gray-100",
  },
  hoverClass: {
    type: String,
    default: "hover:bg-amber-400",
  },
  iconColorClass: {
    type: String,
    default: "text-gray-700",
  },

  /* POZYCJA IKONY */
  iconPosition: {
    type: String,
    default: "left", // left | center
  },
});
</script>
