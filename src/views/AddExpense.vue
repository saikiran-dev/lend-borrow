<template>
  <div class="bg-black">
    <!-- transaction with (user list) , transaction type (Borrows/Lendes), transaction date , reason -->
    <div>
      <label
        for="transaction-with"
        class="block text-sm font-medium text-gray-700"
        >Transaction With</label
      >
      <input
        type="text"
        name="transaction-with"
        id="transaction-with"
        autocomplete="given-name"
        class="mt-1 focus:ring-indigo-500 focus:border-indigo-500 block w-full shadow-sm sm:text-sm border-gray-300 rounded-md"
      />
    </div>
  </div>
</template>
