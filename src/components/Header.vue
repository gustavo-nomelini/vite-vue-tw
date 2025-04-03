<script setup lang="ts">
// Definir props, eventos ou lógica do componente, se necessário
</script>

<template>
  <header class="bg-white border-b border-gray-200 py-4 shadow-sm">
    <div class="container mx-auto px-4 flex flex-col md:flex-row justify-between items-center">
      <div class="mb-4 md:mb-0">
        <h1 class="text-gray-800 text-xl font-semibold">Vue App</h1>
      </div>
      <nav class="mb-4 md:mb-0">
        <ul class="flex space-x-8">
          <li><a href="#" class="text-gray-600 hover:text-indigo-600 font-medium">Início</a></li>
          <li><a href="#" class="text-gray-600 hover:text-indigo-600 font-medium">Recursos</a></li>
          <li>
            <a href="#" class="text-gray-600 hover:text-indigo-600 font-medium">Documentação</a>
          </li>
          <li><a href="#" class="text-gray-600 hover:text-indigo-600 font-medium">Contato</a></li>
        </ul>
      </nav>
      <div>
        <button
          class="bg-indigo-600 text-white px-4 py-2 rounded hover:bg-indigo-700 transition-colors"
        >
          Entrar
        </button>
      </div>
    </div>
  </header>
</template>
