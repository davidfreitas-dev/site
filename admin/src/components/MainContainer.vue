<script setup>
const props = defineProps({
  sidebarWidth: {
    type: String,
    default: '300px'
  }
});
</script>

<template>
  <main class="bg-accent transition-all ease-in-out duration-200 p-5 md:p-8" :style="{ width: `calc(100% - ${sidebarWidth})` }">
    <slot />
  </main>
</template>
