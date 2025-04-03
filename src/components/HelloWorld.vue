<script setup lang="ts">
import { ref } from 'vue';

defineProps<{ msg: string }>();

const count = ref(0);
</script>

<template>
  <h1 class="text-4xl font-bold text-blue-600 mb-6">{{ msg }}</h1>

  <div class="p-6 bg-white dark:bg-gray-800 rounded-lg shadow-md">
    <button
      type="button"
      @click="count++"
      class="px-4 py-2 bg-indigo-600 text-white rounded-md hover:bg-indigo-700 transition-colors"
    >
      count is {{ count }}
    </button>
    <p class="mt-4 text-gray-700 dark:text-gray-300">
      Edit
      <code class="bg-gray-100 dark:bg-gray-700 px-1 py-0.5 rounded text-sm"
        >components/HelloWorld.vue</code
      >
      to test HMR
    </p>
  </div>

  <p class="mt-4 text-gray-600 dark:text-gray-400">
    Check out
    <a
      href="https://vuejs.org/guide/quick-start.html#local"
      target="_blank"
      class="text-indigo-600 hover:underline"
      >create-vue</a
    >, the official Vue + Vite starter
  </p>
  <p class="mt-2 text-gray-600 dark:text-gray-400">
    Learn more about IDE Support for Vue in the
    <a
      href="https://vuejs.org/guide/scaling-up/tooling.html#ide-support"
      target="_blank"
      class="text-indigo-600 hover:underline"
      >Vue Docs Scaling up Guide</a
    >.
  </p>
  <p class="mt-6 text-gray-500 dark:text-gray-500">Click on the Vite and Vue logos to learn more</p>
</template>

<style scoped>
/* Estilos específicos podem ser mantidos aqui, se necessário */
</style>
