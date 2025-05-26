<template>
  <div class="space-y-6">
    <div v-for="(group, index) in groups" :key="index">
      <h2 class="font-bold text-[20px] mb-2">
        foto & kegiatan {{ group.label }}
      </h2>
      <div class="grid grid-cols-4 gap-2 ">
        <div
          v-for="n in group.count"
          :key="n"
          class="w-full h-60 bg-gray-300 rounded "
        />
      </div>
    </div>
  </div>
</template>

<script setup>
const groups = [
  { label: "", count: 5 },
  { label: "1", count: 5 },
  { label: "2", count: 4 },
];
</script>
