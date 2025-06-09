<template>
  <div class="space-y-6">
    <div v-for="(group, index) in groups" :key="index">
      <h2 class="font-bold text-[20px] mb-2">
        foto & kegiatan {{ group.label }}
      </h2>
      <div class="grid grid-cols-4 gap-2">
        <div
          v-for="(foto, i) in group.count"
          :key="i"
          class="w-full h-60 rounded overflow-hidden"
        >
          <img
            :src="foto"
            alt="foto kegiatan"
            class="w-full h-full object-cover"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
const groups = [
  { label: "Arisan PKK", count: ["/4.jpg"] },
  { label: "DAWIS", count: ["/3.jpg"] },
];
</script>
