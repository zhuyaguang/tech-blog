<template>
  <div class="w-full max-w-2xl mx-auto mb-8">
    <input
      type="text"
      v-model="searchQuery"
      @input="$emit('search', searchQuery)"
      placeholder="搜索博客..."
      class="w-full px-4 py-2 rounded-lg border border-gray-300 focus:outline-none focus:ring-2 focus:ring-purple-500"
    />
  </div>
</template>

<script setup>
import { ref } from 'vue';
const searchQuery = ref('');
</script>