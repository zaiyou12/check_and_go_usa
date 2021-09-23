<template>
  <div class="bg-white shadow-lg">
    <div class="bg-black text-white text-xl py-4">{{ title }}</div>
    <ul class="py-4">
      <li class="text-gray-600 px-4 py-3" v-for="(item, index) in body" :key="index">
        {{ item }}
      </li>
    </ul>
  </div>
</template>

<script setup lang="ts">
const props = defineProps<{
  title: string;
  body: Array<string>;
}>();
</script>
