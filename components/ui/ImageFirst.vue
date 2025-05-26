<template>
  <div
    class="w-full h-screen flex items-center justify-center border-2 border-dashed border-gray-300 rounded-lg bg-gray-50"
  >
    <div v-if="!src" class="text-center text-gray-400 text-sm">
      <p>Tidak ada gambar</p>
    </div>
    <img
      v-else
      :src="src"
      alt="Foto"
      class="object-cover w-full h-full rounded-lg"
    />
  </div>
</template>

<script setup>
defineProps({
  src: String,
});
</script>
